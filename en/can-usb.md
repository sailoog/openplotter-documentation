# CAN-USB Stick
---

This chapter is under construction

---

## Warning / Disclaimer

The CAN-USB Stick is a research project on data communication in CAN bus and NMEA 2000® networks (N2K) on boats.

The software is still under development and has not been fully tested. Malfunctions of the CAN-USB Stick and of any connected device might be possible at any time. Manipulating your N2K network could cause damage to connected devices.

Do not rely on data from this device and do not use as primary source for navigation. Liability cannot be accepted for any damages, personal injuries or malfunctions caused by this device.

The CAN-USB Stick is not certified by NMEA.

It is not allowed to use the Actisense® NMEA Reader software for the CAN-USB Stick.

## Overview

The CAN-USB Stick is based on a stm32F103 micro-controller (MCU) connected to a CAN transceiver and is able to read/write on the CAN bus in a boat network. 

The stick works with a CH340 USB to serial converter. Windows 10 does recognize the serial port (no driver is needed). Linux does also support CH340.

N2K network is described in Wikipedia https://en.wikipedia.org/wiki/NMEA_2000

The program of the MCU is re-engineered to work together with CANBOAT project (https://github.com/canboat), which is used by Signal K project (http://signalk.org).
Both packets are used in OpenPlotter project.

The stick does also work with OpenSkipper project (http://openskipper.org).

Not tested:

* MacENC (http://macenc.com)
* PolarView NS (http://www.polarnavy.com)


## Software




## Connection




## Support



