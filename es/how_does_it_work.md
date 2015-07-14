# Cómo funciona

OpenPlotter recopila datos NMEA-0183 desde diferentes fuentes:

* Sensores mediante el puerto GPIO.
* Dispositivos serie USB mediante el puerto USB.
* Cualquier ordenador o dispositivo portátil conectado a la misma red.

Algunas de estas fuentas envían datos NMEA directamente pero otros, como el AIS SDR o el sensor IMU, necesitan ser procesados por OpenPlotter antes de enviar datos NMEA.

Todas estas fuentes son mezcladas en un solo flujo NMEA que es enviado a:

* OpenCPN, para mostrar tu posición sobre la carta.
* Otros dispositivos externos conectados vía WiFi o serie.
* OpenPlotter de nuevo, para calcular nuevas sentencias NMEA.

![](diagram.png)

##Entradas (azul)
* **A**. Datos NMEA de la electrónica de tu barco (GPS, viento, profundidad...).
* **B**. Los datos en bruto del sensor IMU son procesados, convertidos en sentencias NMEA de rumbo magnético y enviados a una entrada UDP localhost 10110 por OpenPlotter. Si hay un barómetro presente, los datos de presión y temperatura serán almacenados.
* **C**. Si OpenPlotter dispone de los datos requeridos, podrá calcular las sentencias NMEA para la declinación magnética, el viento real y el rumbo verdadero. Las nuevas sentencias serán enviadas a la entrada UDP localhost 10110.
* **D**. La señal AIS recibida por el receptor de TDT es decodificada por OpenPlotter. Las sentencias NMEA de AIS serán enviadas a la entrada UDP localhost 10110.
* **E**. If you have an USB GPS dongle, you will have to create a serial input.
* **F**. You can receive NMEA data from any device connected to OpenPlotter by WiFi. You have to create a TCP/UDP input.

##Outputs (green)
* **A**. Multiplexed NMEA stream. All inputs gathered in TCP localhost 10110 output. It is sent to OpenCPN, to external devices and to OpenPlotter for calculations.
* **B**. Orders to autopilot. You have to set a filtered serial output from OpenCPN with autopilot sentences.
* **C**. Remote desktop.
* **D**. Video and audio output by HDMI port. Alternatively, you can get analog video and audio using the composite port.
