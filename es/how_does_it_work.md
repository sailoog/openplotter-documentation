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
* **E**. Si tienes un receptor GPS USB tendrás que crear una entrada serie.
* **F**. Puedes recibir datos NMEA desde cualquier equipo conectado a OpenPlotteír vía WiFi. Tendrás que crear una entrada TCP/UDP.

##Salidas (verde)
* **A**. Flujo de datos NMEA multiplexados. Todas las entradas reunidas en la salida TCP localhost 10110. Es enviado a OpenCPN, a dispositivos externos y a OpenPlotter para cálculos.
* **B**. Órdenes para el piloto automático. Tienes que configurar una salida serie en OpenCPN filtrada con las sentencias para el piloto automático.
* **C**. Escritorio remoto.
* **D**. Salida de video y audio vía puerto HDMI. También puedes obtener video y audio analógico usando el puerto de video y audio compuesto.
