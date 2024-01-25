
weronetzki  on https://forum.arduino.cc/t/conflicitng-declaration-in-adafruit_sensor-esp32-camera/586568/2
juin '20post #2

My quick and dirty way to solve was,

just rename the structure from sensor_t to Adafruit_sensor_t in all related files.
Adafruit_BME280.cpp, Adafruit_BME280.h, Adafruit_Sensor.cpp and Adafruit_Sensor.h

and include all files into your project.

Then change all includes to the two header files to locally (e.g. change
#include <Adafruit_Sensor.h>
to
#include "Adafruit_Sensor.h"
)

That's it
