# 1W temperature sensor

![](DS18B20.png)

You can connect one wire (1W) **DS18B20** sensors to OpenPlotter. This sensor is waterproof and can withstand high temperatures. Connecting multiple DS18B20 in parallel to the same pins, you will be able to get temperature data from coolant engine, exhaust, engine room, fridge, sea ...

## Wiring

Pins names are according to the diagram below.

![](RP2_Pinout.png)

You have to connect these sensors to **GPIO4** (aka GCLK), **GND** and **3.3V** pins. Some sensors may have a fourth wire which do not need to be connected. You need to use a pull-up resistor as shown in the image below. You can connect multiple sensors in paralel using just one resistor.

![](DS18B20_sensors.png)

If you want to change the GPIO pin, edit the file config.txt typing in a terminal:

```sudo nano /boot/config.txt```

At the end of the file you should see a line like this

*dtoverlay=w1-gpio*

replace it by

*dtoverlay=w1-gpio,gpiopin=x*

where x is your desired GPIO pin. Save and reset.

## Settings

See [1W](/1w.md) chapter to configure DS18B20 sensors.