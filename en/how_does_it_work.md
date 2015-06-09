# How does it work?
![](diagram.png)

OpenPlotter collects NMEA data from different sources:

* Sensors through GPIO port.
* Serial devices through USB port.
* Any computer or portable device connected to the same network.

Some of them send NMEA data directly, but others, like SDR AIS or IMU sensor, need to be processed by OpenPlotter before sending NMEA data.

All these sources are combined in a single NMEA stream which is sent to:

* OpenCPN to show your position over the chart.
* Other external devices connected by serial or WiFi.
* OpenPlotter again to calculate new NMEA sentences.

##Inputs
* **A**. NMEA data from your boat equipment (GPS, wind, depth...).
* **B**. Raw data from the IMU sensor is processed, converted to compass NMEA sentences and sent to UDP localhost 10110 input by OpenPlotter. If barometer is present, pressure and temperature data will be logged.
* **C**. If Openplotter has the required data, it will be able to calculate NMEA for magnetic variation, true heading and true wind. The new sentences will be sent to UDP localhost 10110 input.
* **D**. AIS signal from the DVB-T dongle is received and decoded by OpenPlotter. Generated NMEA data is sent to UDP localhost 10110 input.
* **E**. If you have an USB GPS dongle, you will have to create a serial input.
* **F**. You can receive NMEA data from any device connected to OpenPlotter by WiFi. You have to create a TCP/UDP input.

##Outputs
* **A**. Multiplexed NMEA stream. All inputs gathered in TCP localhost 10110 output. It is sent to OpenCPN, to external devices and to OpenPlotter for calculations.
* **B**. Orders to autopilot. You have to set a filtered serial output from OpenCPN with autopilot sentences.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
