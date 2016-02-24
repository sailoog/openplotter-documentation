# ¿Cómo funciona?

OpenPlotter puede obtener datos desde diferentes fuentes:

* Sensores y dispositivos conectados por el puerto GPIO.
* Dispositivos serie conectados por el puerto USB.
* Cualquier ordenador o dispositivo portatil conectado a la intranet.

La mayoria de estas fuentes envian datos directamente en el  formato marino denominado NMEA 0183. Otros, como AIS-SDR o algunos sensores, necesitan ser procesados por OpenPlotter para convertir los datos en bruto a formato NMEA. Por otra parte, existen otros dispositivos que no usan el formato NMEA.

Todas estas fuentes se combinan en un único flujo de datos que puede ser enviados a:

* Internamente, chartplotter (OpenCPN).
* Internamente, calculadora NMEA para generar nuevos datos NMEA.
* Internamente, disparadores/acciones del sistema.
* Otros dispositivos externos desde la intranet o las conexiones serie.
* El inspector de datos.
* El panel virtual de instrumentos.
* Una cuenta de twitter a través de internet.
* Una cuenta de correo elecrónico a través de internet.

A lo largo de los capítulos de este manual iremos viendo como realizar todo esto.

![](diagram.png)
