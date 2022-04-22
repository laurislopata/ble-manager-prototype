# ble-manager-prototype

Setup:

Before scanning for devices, follow the first answer on this stackoverflow post:
https://stackoverflow.com/questions/25427768/bluez-how-to-set-up-a-gatt-server-from-the-command-line
to create a custom Service to check if the phone is discovering them. and when you register the service, one extra step you should do is execute `menu advertise` and `service 0xFFFF` 
in the `bluetoothctl` shell with this the new service will be advertised as well


And when in the app just press "SCAN BLUETOOTH" and when scanning finishes click on your laptops name in the console it will show `Connected to XX:XX:XX:XX:XX:XX` and after this click the other button and it should print the UUIDs of all the services. For me it only prints the default 3: `1800, 1801, 180a` but not `ffff`, and show's error: `Characteristic 0000aaaa-0000-1000-8000-00805f9b34fb not found.`
