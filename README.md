# BluetoothLE

## Description

This a fairly low level testing tool for BLE devices and it's in the form of a Windows app.

## Background

This project has started because I needed a tool to test a BLE device that I was
building.

The best tool I could find was [nRF Connect](https://github.com/NordicSemiconductor/Android-nRF-Connect):
it's a great app, but runs only on mobile.
I didn't have any intentions to dwell hours on the phone so I started out searching
the web for some Python stuff that I could use on the Desktop.
I ended up finding [Pybluez](https://pybluez.github.io/) which seemed a pretty
neat library but it didn't support BLE on Windows yet.
Searching some more, and this time in a programming language closer to Windows,
and I found these [Windows application samples](https://github.com/Microsoft/Windows-universal-samples),
from which I branch from.

The sample was pretty much ready for the the things I needed it for, but it had
some small bugs that I was better off fixing.
Here I fix some bugs and I possibily add some useful stuff to broad its scope of
usage.

## Development and building

This project requires Visual Studio and the Windows Software Development Kit
(SDK) for Windows 10.

## Distributing and packaging

Apart from build and debugging, with Visual Studio you can create an installable
package fot sharing with others, or use to install the app on another computer.
Here are the [istructions](https://docs.microsoft.com/en-us/windows/msix/app-installer/create-appinstallerfile-vs).
The .msixbundle file is what you need.

Installing the package is not as easy as someone would like it to be because
Windows allows side-loading only if it's opted to
(Settings->Update & Security->For Developers).
In addition, you are not allowed to install applications that are not signed,
hence when you build the package make sure you sign it, even if the certificate
you're using is self-signed.
Before you launch the installer add the certificate to the "Trusted People" store.
