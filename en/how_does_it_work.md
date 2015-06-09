# How does it work?
under construction

##Inputs
* **A**. NMEA data from your boat equipment (GPS, wind, depth...).
* **B**. Raw data from the IMU sensor is processed, converted to NMEA  and sent to UDP localhost 10110 by OpenPlotter.
* **C**. If Openplotter has the required data, it will be able to calculate NMEA for Magnetic Variation, True Heading and True Wind.
* **D**. 

##Outputs
* **A**. Multiplexed NMEA stream. All inputs gathered in an output. It is sent to OpenCPN, other external devices and OpenPlotter for calculations.
* **B**. Orders to autopilot. It can be sent to a serial device directly from OpenCPN.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
