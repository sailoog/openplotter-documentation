Qué es OpenPlotter
=======
![OpenPlotter logo](openplotter500x300.png)

Hay gente que compra barcos pero también hay personas que los construyen, ¿porqué no construirte también tu propia electrónca? **OpenPlotter** es una combinación de software y hardware para ser usada como ayuda a la navegación en barcos de pequeña y mediana eslora. Funciona en ordenadores ARM como la [Raspberry Pi](https://www.raspberrypi.org/) y es de código abierto, bajo coste y bajo consumo. Su diseño es modular así que solo tendrás que implementar lo que tu barco necesite. Hazlo tu mismo.

## Características

* **Chartplotter**. Con [OpenCPN](http://opencpn.org), programa de posicionamiento sobre la carta náutica con útiles plugins.
* **Predicciones Meteorológicas**. Descarga y visualiza archivos Grib con [zyGrib](http://www.zygrib.org).
* **Multiplexor NMEA 0183**. Reune y filtra datos precedentes de cualquier número de entradas serie o de red y los envía multiplexados y fultrados a cualquier número de salidas.
* **Signal K (beta)**. OpenPlotter está preparado para [Signal K](http://signalk.org/), el nuevo, formato de intercambio de datos marinos universal, libre y de código abierto.
* **Inspector NMEA**. Comprueba el tráfico de datos para evitar conflictos y solapamientos entre las fuentes.
* **Servidor WiFi NMEA**. Comparte datos NMEA con portátiles, tabletas y teléfonos a bordo o conecta a internet en puerto a través del mismo dispositivo.
* **Escritorio Remoto**. Accede al escritorio de OpenPlotter desde la bañera a través de tus dispositivos móviles.
* **AIS-SDR**. Recibe y decodifica AIS con baratos receptores de TDT. Incluye herramientas de calibración.
* **Declinación Magnética**. Calcula la declinación magnética para le fecha y posición.
* **Compás Electrónico**. Calcula rumbo de aguja con un sensor IMU. Inclinación compensada. Incluye herramientas de calibración.
* **Rumbo Verdadero**. Calcula el rumbo verdadero a partir del rumbo de aguja y la declinación magnética.
* **Viento Real**. Calcula el viento real a partir del viento aparente y la velocidad sobre el agua (corredera) o la velocidad sobre el fondo (GPS).
* ** Barógrafo y Termógrafo **. Desde sensor IMU. Guardar registros cronológicos y muestra gráficos para ver las tendencias.
* **Herramientas de Hora del Sistema**. Establece la hora del sistema a partir de datos NMEA y configura la zona horaria fácilmente.
* **GPSD**. Configura [GPSD](http://www.catb.org/gpsd/).
* **Programas de Inicio**. Configura programas y parametros para ejecutar al inicio.

![OpenPlotter desktop](openplotter.png)