# How does it work?

OpenPlotter can collect data from different sources:

* Sensors and devices connected by GPIO port.
* Serial devices connected by USB port.
* Any computer or portable device connected to the same network.

Most of these sources send NMEA 0183 data directly but others, like SDR AIS or sensors, need to be processed by OpenPlotter to convert raw data to NMEA 0183.

All these sources are combined in a single NMEA data stream which can be sent to:

* Internal chartplotter (OpenCPN).
* Internal  NMEA calculator to create new NMEA data.
* Internal triggers/actions system.
* Other external devices through network or serial connections.
* A twitter account through Internet.
* An e-mail account through Internet.

Besides this, you can connect some common switches, link them to predefined actions and set some outputs to control external devices like relays, LEDs, buzzers, etc.

Through the chapters of this manual we will see how to do this.