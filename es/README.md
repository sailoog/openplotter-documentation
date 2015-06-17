¿Qué es OpenPlotter?
=======
![OpenPlotter logo](openplotter500x300.png)

OpenPlotter es una combinación de software y hardware para ser usada como ayuda a la navegación en barcos de pequeña y mediana eslora. Funciona en ordenadores ARM como la [Raspberry Pi](https://www.raspberrypi.org/) y es de código abierto, bajo coste y bajo consumo. Su diseño es modular así que solo tendrás que implementar lo que tu barco necesite. Hazlo tu mismo.

## Características

* **Chartplotter**. Con [OpenCPN](http://opencpn.org), programa de posicionamiento sobre la carta náutica con útiles plugins.
* **Predicciones meteorológicas**. Descarga y visualiza archivos Grib con [zyGrib](http://www.zygrib.org).
* **Multiplexor NMEA-0183**. Reune datos precedentes de cualquier número de entradas serie o de red y los envía multiplexados a cualquier número de salidas.
* **Inspector NMEA**. Comprueba el tráfico de datos para evitar conflictos y solapamientos entre las fuentes.
* **Servidor WiFi NMEA**. Comparte datos NMEA con portátiles, tabletas y teléfonos a bordo o conecta a internet en puerto a través del mismo dispositivo.
* **Escritorio Remoto**. Accede al escritorio de OpenPlotter desde la bañera a través de tus dispositivos móviles.
* **AIS-SDR**. Recibe y decodifica AIS con baratos receptores de TDT. Incluye herramientas de calibrado.
* **Declinación Magnética**. Calcula la declinación magnética para le fecha y posición.
* **Electronic Compass**. Calculate magnetic heading with an IMU sensor. Tilt compensated. Calibration tools Included.
* **True Heading**. Calculate true heading from magnetic variation and magnetic heading.
* **True Wind**. Calculate true wind from apparent wind and either speed through water (speed log) or speed over ground (GPS).
* **Barograph and Thermograph**. From IMU sensor. Save logs and display graphs to see trends.
* **System Time Tools**. Set the system time from NMEA data and set the time zone easily.
* **GPSD**. Configure [GPSD](http://www.catb.org/gpsd/).
* **Startup Programs**. Select some program parameters to launch at start.

![OpenPlotter desktop](openplotter.png)