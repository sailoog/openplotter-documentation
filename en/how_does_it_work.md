# How does it work?

OpenPlotter can collect data from different sources:

* Sensors and devices connected by GPIO port.
* Serial devices connected by USB port.
* Any computer or portable device connected to the same network.

Most of these sources directly send data in the maritime format called NMEA 0183. Others, like SDR AIS or some sensors, need to be processed by OpenPlotter to convert raw data to NMEA. Finally, there are other devices that do not use NMEA format.

All these sources are combined in a single data stream which can be sent to:

* Internal chartplotter (OpenCPN).
* Internal  NMEA calculator to generate new NMEA data.
* Internal triggers/actions system.
* Other external devices through network or serial connections.
* Data Inspector.
* Virtual Instrument Panel
* A twitter account through Internet.
* An e-mail account through Internet.

Through the chapters of this manual we will see how to do this.

![](diagram.png)