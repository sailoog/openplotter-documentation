# Arduino

Arduino is a board with a mcu. Most of Arduinos or compatible have a mcu with build in adc. They have 8-16 bit adc.

The number of analog inputs channel depend on the mcu

Connected to USB serialport.

In Openplotter we use the firmata script of Arduino IDE.

It communicates with the RPI over firmata protocol.

advantage:

* can be isolated \(by USB to USB isolator, or uart to USB isolator\) 

See [Analog Firmata](/analog-firmata.md)

