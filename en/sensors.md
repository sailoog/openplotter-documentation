## \# Sensors

Some sensors can be connected to the GPIO of the raspberry pi. If these sensors haven't got a connection to the ground of the boat they are safe. When they are grounded you can get ground loops which could demage the raspberry pi or other things. In these situation it is better to use other short mcu boards like arduino and isolate them with an usb to usb isolator for example. 

## I2C

* IMU
* Pressure
* Temperature
* Humidity

![](/assets/screenshot.79.jpg)
## 1W

* [DS18B20](DS18B20.md)

![](/assets/screenshot.80.jpg)
Use add key to add another sensor. Doubleclick the line to edit it.

![](/assets/screenshot.81.jpg)

Use offset to correct value.

If there is a star in signalk name. The text in field Name will replace the star. 



## SPI

The adc \(analog digital converter\) MCP3008 is implemented in openplotter.

![](/assets/screenshot.76.jpg)

It does read voltage between 0 - 3.3V. It is has a 10bit resolution \(0-1023\).

Many signals aren't linear. To get a nearly linear result you can use the value setting.

![](/assets/screenshot.77.jpg)

The medium level in a tank on boats isn't linear to the hight the sensor measures. To calibrate it emty it and insert the adc value for 0%. fill in 10% of max volume and insert adc value and 10.0. Go on untill the tank is full.

Look at the graph you created by clicking on graph

![](/assets/screenshot.78.jpg)

## Pulse

Coming soon

