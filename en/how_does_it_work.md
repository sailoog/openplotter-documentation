# How does it work?

OpenPlotter collects data from different sources:

* Sensors through GPIO port.
* Serial devices through USB port.
* Any computer or portable device connected to the same network.

Most of these sources send NMEA 0183 data directly, but others, like SDR AIS or sensors, need to be processed by OpenPlotter to convert data to NMEA 0183.

All these sources are combined in a single NMEA 0183 data stream which is sent to:

* OpenCPN.
* Other external devices through network or serial connections.
* OpenPlotter again to calculate new NMEA 0183 data.
