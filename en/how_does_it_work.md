# How does it work?
under construction

##Inputs
* **A**. NMEA data from your boat equipment (GPS, wind, depth...).
* **B**. Raw data from the IMU sensor is processed, converted to Compass NMEA data  and sent to UDP localhost 10110 input by OpenPlotter. If barometer is present, weather data will be logged.
* **C**. If Openplotter has the required data, it will be able to calculate NMEA for Magnetic Variation, True Heading and True Wind. The new sentences will be sent to UDP localhost 10110 input.
* **D**. AIS signal from the DVB-T dongle is received and decoded by OpenPlotter. Generated NMEA data is sent to UDP localhost 10110 input.
* **E**. If you have an USB GPS dongle, you will have to create a serial input.

##Outputs
* **A**. Multiplexed NMEA stream. All inputs gathered in an output. It is sent to OpenCPN, other external devices and OpenPlotter for calculations.
* **B**. Orders to autopilot. It can be sent to a serial device directly from OpenCPN.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
