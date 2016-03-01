# ¿Qué es OpenPlotter?

![OpenPlotter logo](../en/openplotter500x300.png)


Hay gente que compra barcos pero también hay personas que los construyen, ¿por qué no construirte tu própia electrónica también? OpenPlotter es una combinación de software y hardware para ser usado como ayuda a la navegación en barcos de pequeña y mediana eslora. Es también un completo sistema de domótica a bordo. Funciona en ordenadores ARM como la [Raspberry Pi](https://www.raspberrypi.org/) y es de código abierto, bajo coste y bajo consumo. Su diseño es modular, así que solo tienes que incorporar lo que tu barco necesite. !Hazlo tu mismo!.


## Características

* **Chartplotter**. Con [OpenCPN](http://opencpn.org), un programa de navegación, con útiles plugins.
* **Predicciones Metereológicas**. Descarga y visualiza ficheros GRIB mediante [zyGrib](http://www.zygrib.org).
* **Multiplexor NMEA 0183**. Combina y filtra datos procedentes de cualquier número de entradas serie o de red.  Envía y filtra a cualquier número de salidas.
* **Signal K (beta)**. OpenPlotter está preparado para [Signal K](http://signalk.org/), el nuevo formato de intercambio de datos marinos, libre y de código abierto.
* **Inspector**. Comprueba el tráfico de datos, para evitar conflictos y solapamientos entre dos fuentes.
* **Punto de acceso WiFi**. Comparte datos (NMEA 0183, Signal K, escritorio remoto, conexión Internet) con los portátiles, tabletas y teléfonos a bordo. Conecta a internet en el puerto a través del mismo dispositivo.
* **Escritorio Remoto**. Accede al escritorio de OpenPlotter desde la bañera a través de tus dispositivos móviles.
* **Sin monitor**. Posibilidad de uso sin monitor, fácilmente.
* **AIS-SDR**. Recibe y decodifica AIS mediante asequibles receptores de TDT. Incluye herramientas de calibración.
* **Brújula electronica y Escora**. Lee el rumbo de aguja y la escora desde el sensor IMU. Inclinación compensada. Incluye herramientas de calibración.
* **Barógrafo, Termógrafo e Higrógrafo**. Gracias a sensores de presión atmosférica, temperatura y humedad. Guarda registros y muestra gráficos para ver la tendencia.
* **Múltiples sensores de temperatura**. Obtiene datos del refrigerante del motor, el tubo de escape, nevera, agua del mar, etc...
* **Sensores Especiales**. Detecta apertura de puertas/ventanas, niveles en depósitos y sentinas, movimientos de personas...
* **Declinación Magnética**. Calcula la declinación magnética para una fecha y posición dadas.
* **Rumbo verdadero**. Calcula el rumbo verdadero a partir de la declinación magnética y del rumbo de aguja.
* **Viento Real**. Calcula el viento real a partir del viento aparente y o bien la velocidad sobre el agua (corredera) o la velocidad sobre el fondo (GPS).
* **Ratio de Giro**. Calcula la velocidad a la que el barco está girando.
* **Monitorización Remota**. Publica datos en Twitter o los envía por correo electrónico.
* **Sistema de Acciones**. Compara un valor configurable con cualquier dato que fluya a través del sistema y lo utiliza como detonante de múltiples acciones predefinidas.
* **Interruptores Configurables**. Conecta interruptores externos y los vincula a acciones.
* **Activa Dispositivos Externos**. Relés, LEDs, zumbadores ...
* **Herramientas de Hora del Sistema**. Establece la fecha y hora del sistema a partir de datos NMEA y configura la zona horaria fácilmente.
* **Programas de Inicio**. Configura programas y parámetros para ejecutar al inicio.

![OpenPlotter desktop](../en/openplotter.png)