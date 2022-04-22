# ble-manager-prototype

Setup:

Before scanning for devices, follow the first answer on this stackoverflow post:
https://stackoverflow.com/questions/25427768/bluez-how-to-set-up-a-gatt-server-from-the-command-line
to create a custom Service to check if the phone is discovering them. and when you register the service, one extra step you should do is go to `menu advertise` and `service 0xFFFF` 
in the `bluetoothctl` shell with this the new service will be advertised as well
