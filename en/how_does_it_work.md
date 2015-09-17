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


## How data flows and connections
![](diagram.png)

### Inputs (blue)
* **A**. Data from your boat equipment (GPS, wind, depth...).
* **B**. Raw data from sensors is processed, converted to NMEA 0183 and sent to system input UDP localhost 10110.
* **C**. If Openplotter has the required data, it will be able to calculate magnetic variation, true heading and true wind. The new NMEA 0183 data will be sent to system input UDP localhost 10110.
* **D**. AIS signal from the DVB-T dongle is received and decoded by OpenPlotter. Generated NMEA 0183 data is sent to system input UDP localhost 10110.
* **E**. USB GPS dongles send NMEA 0183. You will have to create a serial input in the NMEA 0183 multiplexer.
* **F**. You can get NMEA 0183 data from any device connected by WiFi or ethernet. You will have to create a network input in the NMEA 0183 multiplexer.

### Outputs (green)
* **A**. Multiplexed NMEA 0183 stream. All inputs gathered in system outout TCP localhost 10110. It is sent to OpenCPN, to external devices and to OpenPlotter for new calculations.
* **B**. Orders to autopilot. You have to set a filtered serial output from OpenCPN with autopilot NMEA 0183 sentences.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
