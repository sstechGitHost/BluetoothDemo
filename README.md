# BluetoothDemo
Sample Xamarin.Android app for bluetooth interaction between devices

This is Xamarin Android solution demonstrates how to connect to bluetooth devices (not low energy devices) 

What BluetoothActivity class does?

1) Creates BluetoothAdapter instance
2) Checks if BluetoothAdapter is null
3) Checks if its enabled or not
4) The scan button starts the discovery of bluetooth devices by calling, BluetoothAdapter.StartDiscovery() method
5) The class has registered itself with a broadcast receiver class, Receiver
6) Whenever a bt devices is discovered,  BluetoothDevice.ActionFound action is raised which is found in the Receiver class
7) In the Receiver, the  BluetoothDevice.ActionFound can be traced and all found devices can be added to a list adapter

