# CAN-USB Stick
---

This chapter is under construction

---

![](n2k_b.jpg)

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


## Connection

![](n2k_a.jpg)
Example of a small N2K Network

The backbone (or trunk) starts with a 120Ω terminator   and ends with a 120Ω terminator. The two resistors are working in parallel, so the resistance is $$120Ω/2=60Ω$$. If there is a broken connection in the backbone you can measure only 120Ω or nothing but not 60Ω. That is a very easy way to check the bus.

The drop line to the devices should not be longer than 6 m. The backbone can have 100m in length.

The CAN-USB Stick is not isolated, so connecting the Raspberry Pi power supply to the CAN bus power supply is highly recommended.

## Software









## Support



