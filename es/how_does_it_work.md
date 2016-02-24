# ¿Cómo funciona?

OpenPlotter puede obtener datos desde diferentes fuentes:

* Sensores y dispositivos conectados por el puerto GPIO.
* Dispositivos serie conectados por el puerto USB.
* Cualquier ordenador o dispositivo portatil conectado a la misma red.

La mayoria de estas fuentes envian datos directamente en el  formato marino denominado NMEA 0183. Otros, como AIS-SDR o algunos sensores, necesitan ser procesados por OpenPlotter para convertir los datos en bruto a formato NMEA. Por otra parte, existen otros dispositivos que no usan el formato NMEA.

Todas estas fuentes se combinan en un único flujo de datos que puede ser enviados a:

* Internal chartplotter (OpenCPN).
* Internal  NMEA calculator to generate new NMEA data.
* Internal triggers/actions system.
* Other external devices through network or serial connections.
* Data Inspector.
* Virtual Instrument Panel
* A twitter account through Internet.
* An e-mail account through Internet.

Through the chapters of this manual we will see how to do this.

![](diagram.png)
