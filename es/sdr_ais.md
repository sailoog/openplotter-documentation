# DVB-T dongle (AIS)

Los receptor de TDT USB basados en el chip Realtek RTL2832U y en el nuevo sintonizador R820T2, pueden funcionar como receptores AIS SDR. OpenPlotter viene preparado de serie para recibir AIS SDR, simplemente tienes que calibrarlo.

A DVB-T dongle will need more power than the Raspberry Pi USB port can provide. You need to plug the dongle into a powered USB hub.

You can buy our DVB-T dongle and we can calibrate it for you and include a note with the gain and correction value (ppm):
Opcionalmente podemos calibrarlos por ti y añadir una nota con el valor de corrección (ppm).
http://www.sailoog.com/shop-category/openplotter

or you can follow this detailed guide:

http://sailoog.dozuki.com/Guide/Connecting+and+calibrating+SDR-AIS+dongles/3

## Receiving
![](sdr_ais1.jpeg)

Once you have found your **gain** and **correction** value (in red), select ***Enable AIS NMEA generation*** (in pink).

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