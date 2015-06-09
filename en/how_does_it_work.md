# How does it work?
![](diagram.png)

Basically, OpenPlotter collects NMEA data from different sources:
* Sensors trough GPIO port. Openplotter process raw data and create NMEA sentences.
* Serial devices trough USB. Some of then, like RS422 coverters or GPS, directly send NMEA data but there are some that need to be processed by openPlotter before sending NMEA data, like DVB-T SDR AIS receptor.
* Network devices. From any computer or portable device.

It gathers all this data in one unique stream which is sent to:

* OpenCPN to show our boat over the chart and to other devices connected by serial or 
* 

##Inputs
* **A**. NMEA data from your boat equipment (GPS, wind, depth...).
* **B**. Raw data from the IMU sensor is processed, converted to Compass NMEA data  and sent to UDP localhost 10110 input by OpenPlotter. If barometer is present, weather data will be logged.
* **C**. If Openplotter has the required data, it will be able to calculate NMEA for Magnetic Variation, True Heading and True Wind. The new sentences will be sent to UDP localhost 10110 input.
* **D**. AIS signal from the DVB-T dongle is received and decoded by OpenPlotter. Generated NMEA data is sent to UDP localhost 10110 input.
* **E**. If you have an USB GPS dongle, you will have to create a serial input.
* **F**. You can receive NMEA data from any device connected to OpenPlotter by WiFi. You have to create a TCP/UDP input.

##Outputs
* **A**. Multiplexed NMEA stream. All inputs gathered in an output. It is sent to OpenCPN, other external devices and OpenPlotter for calculations.
* **B**. Orders to autopilot. It can be sent to a serial device directly from OpenCPN.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
