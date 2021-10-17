# Bluetooth Low Energy sample

Shows how to use the Windows Bluetooth LE APIs to act either as a BLE client or server. 

## Client

Shows how to act as a client to communicate with a Bluetooth Low Energy (LE) device
using the Bluetooth GATT protocol. Acts as a GATT client to access nearby GATT servers like
heart rate sensors or temperature sensors.

Specifically, this sample shows how to:

- Enumerate nearby Bluetooth LE devices
- Query for supported services
- Query for supported characteristics
- Read and write data
- Subscribe to indicate and notify events

## Server
As of build 15003 and above, Bluetooth LE GATT Server APIs are available.
This sample can be used to advertise support for CalcService - a custom service that allows a remote client to write to two operand characteristics
and an operator and read the result. 

This samples shows how to:
- Initialize and publish a custom service/characteristic hierarchy 
- Implement event handlers to handle incoming read/write requests
- Notify connected clients of a characteristic value change

## More Details
Search for "BT_Code" to find the portions of the sample that are particularly
relevant to Bluetooth.
Note in particular the "bluetooth" capability declaration in the manifest.

**Note** The Windows universal samples require Visual Studio to build and Windows 10 to execute.

To obtain information about Windows 10 development, go to the [Windows Dev Center](http://go.microsoft.com/fwlink/?LinkID=532421)

To obtain information about Microsoft Visual Studio and the tools for developing Windows apps, go to [Visual Studio](http://go.microsoft.com/fwlink/?LinkID=532422)

### Reference

[Windows.Devices.Bluetooth namespace](https://msdn.microsoft.com/library/windows/apps/windows.devices.bluetooth.aspx)

[Windows.Devices.Bluetooth.GenericAttributeProfile namespace](https://msdn.microsoft.com/library/windows/apps/windows.devices.bluetooth.genericattributeprofile.aspx)

[Windows.Devices.Enumeration namespace](https://msdn.microsoft.com/library/windows/apps/windows.devices.enumeration.aspx)

### Conceptual

* Documentation
  * [Bluetooth GATT Client](https://msdn.microsoft.com/windows/uwp/devices-sensors/gatt-client)
  * [Bluetooth GATT Server](https://msdn.microsoft.com/windows/uwp/devices-sensors/gatt-server)
  * [Bluetooth LE Advertisements](https://docs.microsoft.com/windows/uwp/devices-sensors/ble-beacon)
* [Windows Bluetooth Core Team Blog](https://blogs.msdn.microsoft.com/btblog/)
* Videos from Build 2017
  * [Introduction to the Bluetooth LE Explorer app](https://channel9.msdn.com/Events/Build/2017/P4177)
    * [Source code](https://github.com/Microsoft/BluetoothLEExplorer)
    * [Install it from the Microsoft Store](https://www.microsoft.com/store/apps/9n0ztkf1qd98)
  * [Unpaired Bluetooth LE Device Connectivity](https://channel9.msdn.com/Events/Build/2017/P4178)
  * [Bluetooth GATT Server](https://channel9.msdn.com/Events/Build/2017/P4179)

## System requirements

**Client:** Windows 10 Anniversary Edition

**Server:** Windows Server 2016 Technical Preview

**Phone:** Windows 10 Anniversary Edition

## Build the sample

1. Double-click the Visual Studio Solution (.sln) file.
2. Press Ctrl+Shift+B, or select **Build** \> **Build Solution**.

## Run the sample

The next steps depend on whether you just want to deploy the sample or you want to both deploy and run it.

### Deploying the sample

- Select Build > Deploy Solution. 

### Deploying and running the sample

- To debug the sample and then run it, press F5 or select Debug >  Start Debugging. To run the sample without debugging, press Ctrl+F5 or selectDebug > Start Without Debugging. 
