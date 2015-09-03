# DVB-T dongle (AIS)

Los receptores de TDT USB basados en el chip Realtek RTL2832U y en el nuevo sintonizador R820T2, pueden funcionar como receptores AIS SDR. OpenPlotter viene preparado de serie para recibir AIS SDR, simplemente tienes que calibrar el receptor.

Este dispositivo necesitará más corriente de la que la Raspberry Pi le puede suministrar asi que tendrás que conectarlo a un Hub USB auto-alimentado.

Puedes comprar nuestro receptor TDT. Opcionalmente podemos calibrarlo por ti y añadir una nota con el valor de ganancia y de corrección (ppm):

http://www.sailoog.com/shop-category/openplotter

o puedes seguir esta guía detallada:

http://sailoog.dozuki.com/Guide/Connecting+and+calibrating+SDR-AIS+dongles/3

## Recibir
![](sdr_ais1.jpeg)

Una vez has encontrados tus valores de **ganancia** y de **corrección** (en rojo), selecciona **Activar generación NMEA AIS** (en rosa).

![](sdr_ais2.jpeg)

If you have AIS traffic around, AIS NMEA data will be decoded and sent to **UDP localhost 10110 input** (in orange).

If you want to have access to AIS data you will have to connect your software (OpenCPN) to **TCP localhost 10110 output** (in yellow).

Press **Restart** (in red) to be sure the multiplexer is working.

Press **Show output** (in pink) to see AIS data in the NMEA Inspector.

![](sdr_ais3.jpeg)

![](sdr_ais4.jpeg)

Be sure OpenCPN is listening to **TCP localhost 10110** (in yellow).

## Antena

Aunque puedes llegar a recibir algún barco con la mini antena suministrada, esta no es suficiente para la óptima recepción de las frecuencias AIS. Cualquier antena VHF con el adaptador de conexión adecuado funcionará correctamente. El tipo de conexión de antena del dispositivo es MCX hembra.

Algunas antenas para auto-construcción:

http://sdrformariners.blogspot.com.es/p/blog-page.html

http://nmearouter.com/docs/ais/aerial.html

https://www.youtube.com/watch?v=SdEglNHyHB4