# libDHT - yet anothe DHT lib
Arduino compatible DHT 11/22, AM2302 lib with dewpoint, heat-index and other goodies. 

##Features

1. Autodetection of sensor type
2. Read humidity and temperature in one function call.
3. Determine heat index in *C or *F
4. Determine dewpoint with various algorithms(speed vs accuracy)
5. Determine thermal comfort
  * Empiric comfort function based on comfort profiles
  * Multiple comfort profiles. Default based on http://epb.apogee.net/res/refcomf.asp
  * Determine if it's too cold, hot, humid, dry, based on current comfort profile
6. Optimized for sensor read speed(~5ms for DHT22), stack and code size.

## Statistics

Platform| 				SensorReading(ms)| 	DewPoint-Accurate&Fast(ms)
|						(CPU speed should not matter here)|	
ESP8266-ESP12 @ 80Mhz|	5.6ms|					0.5ms	


## Credits

Based on *DHT-sensor-library* https://github.com/adafruit/DHT-sensor-library
Based on *arduino-DHT* https://github.com/markruys/arduino-DHT
Based on *DHTlib* https://github.com/RobTillaart/Arduino/tree/master/libraries/DHTlib

**This was tested on an ESP8266 module(ESP-12) running at 80Mhz.**

**_This is in theory compatible with Arduino but untested..._**

If you own an Arduino and want to help with testing, open an issue and let me know.
