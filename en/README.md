# What is OpenPlotter?

---

**This chapter needs to be written/updated/translated**

[http://forum.openmarine.net/forumdisplay.php?fid=16](http://forum.openmarine.net/forumdisplay.php?fid=16)

---

![OpenPlotter logo](openplotter500x300.png)

There are people who buy boats but there are also people who build them, why not build your own electronics too? OpenPlotter is a combination of software and hardware to be used as navigational aid on small and medium boats. It is also a complete home automation system onboard. It works on ARM computers like the [Raspberry Pi](https://www.raspberrypi.org/) and is open-source, low-cost and low-consumption. Its design is modular, so you just have to implement what your boat needs. Do it yourself.

## Features

* **Chartplotter**. With [OpenCPN](http://opencpn.org), a navigation software with useful plugins.
* **Weather Forecast**. Download and visualize GRIB files with [zyGrib](http://www.zygrib.org).
* **NMEA 0183 Multiplexer**. Multiplex and filter data inputs from any number of serial and network interfaces. Send and filter to any number of outputs.
* **SignalK**. OpenPlotter uses SignalK as the base protocol to interact between different networks. Input data has to be converted into SignalK. SignalK data can be converted to NMEA networks.
* **Diagnostic**. Checks the data traffic of NMEA0183 input and output. On Signal K it is a kind of data explorer.
* **WiFi Access Point, Ethernet, GSM**. Share data \(NMEA 0183, Signal K, remote desktop, Internet connection, gofree\) with laptops, tablets and phones on board. Connect to internet on port through the same device.
* **Remote Desktop**. Access to OpenPlotter desktop from the cockpit through your mobile devices.
* **Headless**. Easy start without monitor.
* **SDR-AIS**. Receive and decode AIS with cheap DVB-T dongles. Calibration tools Included.
* **Electronic Compass and Heel**. Read magnetic heading and heel angle from an IMU sensor. Tilt compensated. Calibration tools Included.
* **Barograph, Thermograph and Hygrograph**. From pressure, temperature and humidity sensors.
* **Multiple temperature sensors**. Get data from coolant engine, exhaust, fridge, sea...
* **Special Sensors**. Detect opening doors, windows, tank level, human body motion...
* **Wireless Sensors**. Detect temperature, humidity, ...
* **Analog Sensors**. To read voltage, amperage, resistance. Shows Battery status, power consumption, tank level...
* **Magnetic Variation**. Calculate magnetic variation for date and position.
* **True Heading**. Calculate true heading from magnetic variation and magnetic heading.
* **True Wind**. Calculate true wind from apparent wind and either speed through water \(speed log\) or speed over ground \(GPS\).
* **Rate Of Turn**. Calculate the rate the ship is turning.
* **Remote Monitoring**. Publish data on Twitter or send it by email.
* **Actions System**. Compare a custom value with any data flowing through your system and use it as a trigger to run multiple predefined actions.
* **Custom Switches**. Connect external switches and link them with actions.
* **Handle External Devices**. Relays, LEDs, buzzers ...
* **System Time Tools**. Set the system time from NMEA data and set the time zone easily.
* **Tools**. Integration of self programmed modules and advanced feature modules.
* **Startup Programs**. Select some program parameters to automatically launch at start.

![](openplotter.jpg)



