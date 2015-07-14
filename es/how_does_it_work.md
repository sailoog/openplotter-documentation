# Cómo funciona

OpenPlotter recopila datos NMEA-0183 desde diferentes fuentes:

* Sensores mediante el puerto GPIO.
* Dispositivos serie USB mediante el puerto USB.
* Cualquier ordenador o dispositivo portátil conectado a la misma red.

Algunas de estas fuentas envían datos NMEA directamente pero otros, como el AIS SDR o el sensor IMU, necesitan ser procesados por OpenPlotter antes de enviar datos NMEA.

All these sources are combined in a single NMEA stream which is sent to:

* OpenCPN to show your position over the chart.
* Other external devices connected by serial or WiFi.
* OpenPlotter again to calculate new NMEA sentences.

![](diagram.png)

##Inputs (blue)
* **A**. NMEA data from your boat equipment (GPS, wind, depth...).
* **B**. Raw data from the IMU sensor is processed, converted to compass NMEA sentences and sent to UDP localhost 10110 input by OpenPlotter. If barometer is present, pressure and temperature data will be logged.
* **C**. If Openplotter has the required data, it will be able to calculate NMEA for magnetic variation, true heading and true wind. The new sentences will be sent to UDP localhost 10110 input.
* **D**. AIS signal from the DVB-T dongle is received and decoded by OpenPlotter. Generated NMEA data is sent to UDP localhost 10110 input.
* **E**. If you have an USB GPS dongle, you will have to create a serial input.
* **F**. You can receive NMEA data from any device connected to OpenPlotter by WiFi. You have to create a TCP/UDP input.

##Outputs (green)
* **A**. Multiplexed NMEA stream. All inputs gathered in TCP localhost 10110 output. It is sent to OpenCPN, to external devices and to OpenPlotter for calculations.
* **B**. Orders to autopilot. You have to set a filtered serial output from OpenCPN with autopilot sentences.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
