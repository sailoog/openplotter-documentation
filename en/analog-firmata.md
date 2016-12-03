# Analog Firmata

An Arduino, Teensy or STM32 boards which can be programed by Arduino IDE or which have a library for standard firmata are useable.

The communication is done with USB port or an USB to serial converter. We recommend to use an isolator when using analog signals \(usb to usb isolator or uart to USB isolator or use an ADUM1201 and a simple uart to serial converter \).

When firmata standard is installed. Ad the new USB port in USB manager. **The name of the port has to be ttyOP-FIRM!**

Next step is edditing the configuration file.

Analog Firmata can be started. Best way to see if connecting works is to start openplotter from a terminal session.

The start of pymata takes some seconds.

The configuration file is the same one which is used by [ads1115.](/analog-ads1115.md)

There are up to 16 sections \(\[FIRMATA\_0\]..\[FIRMATA\_15\]\)

Example:

_\[FIRMATA\_1\]   
sk\_name = tanks.fuel.right.currentLevel   
adjust\_points = \[\[52.0,0.0\],\[522.0,25.0\],\[708.0,50.0\],\[913.0,100\],\[1024.0,100.01\]\]_

