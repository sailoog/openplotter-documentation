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


## how data flows and connections
![](diagram.png)

### Inputs (blue)
* **A**. Data from your boat equipment (GPS, wind, depth...).
* **B**. Raw data from sensors is processed, converted to NMEA 0183 and sent to system input UDP localhost 10110.
* **C**. If Openplotter has the required data, it will be able to calculate NMEA for magnetic variation, true heading and true wind. The new sentences will be sent to UDP localhost 10110 input.
* **D**. AIS signal from the DVB-T dongle is received and decoded by OpenPlotter. Generated NMEA data is sent to UDP localhost 10110 input.
* **E**. If you have an USB GPS dongle, you will have to create a serial input.
* **F**. You can receive NMEA data from any device connected to OpenPlotter by WiFi. You have to create a TCP/UDP input.

### Outputs (green)
* **A**. Multiplexed NMEA stream. All inputs gathered in TCP localhost 10110 output. It is sent to OpenCPN, to external devices and to OpenPlotter for calculations.
* **B**. Orders to autopilot. You have to set a filtered serial output from OpenCPN with autopilot sentences.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
