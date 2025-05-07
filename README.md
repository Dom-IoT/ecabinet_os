### eCabinet - Operating System
The operating system for the eCabinet project. This OS is developed onto a m5stack device.

Connections for M5Stack Demo Board :

RFID : 21-SDA 22-SCL

MATRIX : 12-SIGNAL

SENSOR : DIGITAL-2 ANALOG-35

### Requirements
Use platformio to build and push code to the board, change wifi.cpp file by setting your own wifi id and password, change mqtt.cpp and edit IPAddress server_mqtt(192,168, 113, 32) by setting the IP with IP of your device.

On the VM Debian where your Home Assistant instance is installed, go to configuration -> network -> and add a port forwarding : (name : MQTT), Host Port : 1883, IP guest : 10.0.2.15, Guest port : 1883