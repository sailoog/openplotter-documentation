# How does it work?

OpenPlotter can collect data from different sources:

* Sensors and devices connected to GPIO port.
* Serial devices connected to USB port.
* Other devices connected to USB port
* Any computer or portable device connected to the same network.

Most of these sources directly send data in the maritime format called NMEA 0183 or NMEA 2000. The problem is that NMEA 0183 can't communicate with NMEA 2000. So we use the free maritime communication SignalK. Both NMEA formats can communicate to SignalK.

Other devices, like SDR AIS, ADC, GPIO or some sensors, need to be processed by OpenPlotter to convert raw data to NMEA or SignalK.

All these sources are combined in data streams which can be sent to SignalK, because this is openplotter base protocol since 0.9.0:

The soft- and hardware needs different data streams

1. the good old **NMEA 0183**

2. the CAN-BUS network \(standard bus-system in cars\) with the special **NMEA 2000** protocol

3. **SignalK** browser optimized protocol

4. trigger\/action system


NMEA 0183 is used for:

* most pc, tablets and mobile software at the moment as the Internal chartplotter \(OpenCPN\).
* missing sentences can be converted from SignalK to NMEA 0183 with Openplotter tools.

NMEA 2000 is used in:

* most modern boats \(plotter, engine, ...\)
* very little software.

SignalK is used for:

* future software as it is optized for internet browser
* Virtual Instrument Panel
* has a readable protocol where additions can be done
* can receive NMEA 2000, NMEA 0183 and SignalK

trigger\/action system for:

* warning, information, energie saving, automation, ...
* can use twitter, e-mail, mqtt

Through the chapters of this manual we will see how to do this.
![](diagram.png)

