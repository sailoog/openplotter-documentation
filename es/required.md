# Requerido

##Ordenador embebido ARM
![](rpi2.jpg)

En estos momentos recomendamos la popular [Raspberry Pi 2 Model B](https://www.raspberrypi.org/products/raspberry-pi-2-model-b/) porque reúne los requisitos: bajo coste, bajo consumo y tiene una enorme comunidad de desarrolladores.

¡**OpenPlotter RPI**,  el sistema operativo para Raspberry Pi y OpenPlotter está listo!

##Caja
![](box.png)

Existen un montón de modelos para proteger la placa Raspberry Pi.
**Estamos trabajando en una caja resistente al agua.**

##Fuente de alimentación y cableado
![](power.png)

La Raspberry se alimenta con una fuente de 5V mediante un conector micro USB (como la mayoría de cargadores de teléfono móvil estándar). La corriente que necesite (mA) dependerá de lo que conectemos a la placa. Para su funcionamiento interno puede llegar a consumir hasta 500mA y el máximo que puede gestionar vía USB son 1000mA por lo que necesitaremos como mínimo un cargador capaz de servir entre 1,5A y 2A. Si necesitamos conectar dispositivos USB que consuman más de 1A en total, tendremos que usar un Hub USB externo auto-alimentado.

Una buena opción podría ser un adaptador de coche (12v a 5V, 3.1A) con dos salidas por si necesitamos alimentar también un Hub USB.

##Monitor HDMI/DVI/VGA/TV y cableado
![](hdmi.png)

####HDMI

La Raspberry Pi tiene un puerto HDMI (video+audio) que puedes conectar a cualquier monitor o TV compatible con el cable correspondiente. Esta es la opción de más calidad y fácil ya que la mayoría de monitores y TV modernas tienen este tipo de conexión. También existen otras alternativas:

####DVI

Para monitores con entrada DVI, tendrás que usar un cable HDMI-DVI.

####VGA 

Pra monitores con entrada VGA, tendrás que usar un adaptador HDMI-VGA. Recomendamos usar solo adaptadores auto-alimentados.

####Video compuesto

Para TV analógicas tendremos que usar la salida de video/audio de 3.5mm de video compuesto de la Raspberry. Esta es la opción de menos calidad. También podremos usar esta salida de audio y la de video HDMI simultaneamente.

##Keyboard and mouse
![](keyboard.png)

Any standard USB keyboard and mouse will work with your Raspberry Pi. Wireless keyboards and mice will work if already paired.

##SD card
![](sd.png)

The Raspberry Pi 2 should work with any micro-SD-compatible cards, although there are some guidelines that should be followed:

####SD card size (capacity) 

A minimum of 4GB is required but 8GB is recommended.

####SD card class

The card class determines the sustained write speed for the card; a class 4 card will be able to write at 4MB/s, whereas a class 10 should be able to attain 10 MB/s. However it should be noted that this does not mean a class 10 card will outperform a class 4 card for general usage, because often this write speed is achieved at the cost of read speed and increased seek times.

####Buy a SD card with OpenPlotter RPI pre-installed
8GB class 6 microSD card (with a full-size SD adaptor) that outperforms almost all other SD cards on the market.

http://www.sailoog.com/shop-category/openplotter

##OpenPlotter RPI "the software"
![](openplotter_rpi.png)

####Download
http://www.sailoog.com/blog-categories/openplotter-download