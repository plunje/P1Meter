# P1-Meter-ESP8266
Software for the ESP2866 that posts P1 smart meter data to custom API Endpoint (with CRC checking and OTA firmware updates)

### Installation instrucions
- Make sure that your ESP8266 can be flashed from the Arduino environnment: https://github.com/esp8266/Arduino
- Install the SoftSerial library from: https://github.com/plerup/espsoftwareserial
- Place all files from this repository in a directory. Open the .ino file.
- Adjust WIFI, API Endpoint in parameters.h
- Compile and flash

### Connection of the P1 meter to the ESP8266
You need to connect the smart meter with a RJ11 connector. This is the pinout to use
![RJ11 P1 connetor](http://gejanssen.com/howto/Slimme-meter-uitlezen/RJ11-pinout.png)

Connect GND->GND on ESP, RTS->3.3V on ESP and RxD->any digital pin on ESP. In this sketch I use D5
