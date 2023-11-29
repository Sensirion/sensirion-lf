## Experimental Arduino library for Sensirion liquid flow sensors 

[![Build Status](https://travis-ci.org/winkj/sensirion-lf.svg?branch=master)](https://travis-ci.org/winkj/sensirion-lf)

This is an Arduino library for the Sensirion Liquid Flow sensors, based on the
github snippet page at https://github.com/Sensirion/arduino-liquid-flow-snippets
and the documentation on https://developer.sensirion.com/archive/tutorials/arduino-interface-for-liquid-flow-sensors/ .

### Supported sensors
Currently, the following sensors are supported:
- SLF3X

The following sensors are expected to work, but haven't been tested:
- LD20

## Included examples

### slf3x-minimal

This is a minimal example, reading out the data from the sensor and printing
it to the serial console. Use the Arduino IDE's "Serial Monitor" to see the
values read from the sensor

### slf3x-demo

This example adds a second output format that is suitable for the plotter that
is integrated with the Arduino IDE. To enable that format, simply uncomment the
```#define GENERATE_PLOTTER_OUTPUT``` line. Note that the code will scale the
flow values by a factor of 1000 which changes the unit of the output to
micro liters per hour; this is done to get the values into a similar range as
the temperature read from the sensor.

The plot should look similar to this:

![SLF3X plot](/doc/sensirion-lf-plot.jpg)



### Feedback
If you have questions or suggestions, please submit an issue via github.
