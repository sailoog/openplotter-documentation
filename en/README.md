What is OpenPlotter?
=======

OpenPlotter is a combination of software and hardware to be used as navigational aid on small and medium boats. It works on ARM computers like the [Raspberry Pi](https://www.raspberrypi.org/) and is open-source, low-cost and low-consumption. Its design is modular, so you just have to implement what your boat needs. Do it yourself.

## Features

* **Chartplotter**. With [OpenCPN](http://opencpn.org), a chartplotter and GPS navigation software.
* **Weather forecast**. Download and visualize GRIB files with [zyGrib](http://www.zygrib.org).
* **NMEA-0183 Multiplexer**. Multiplexe data inputs from any number of serial lines and network interfaces and send to any number of outputs.
* NMEA inspector
* WiFi NMEA server/client through the same device
* Remote desktop
* SDR-AIS receiver and decoder. Calibration tools.
* Calculate magnetic variation for date and position
* Calculate True Wind
* Calculate True Heading
* Electronic compass from IMU sensor. Tilt compensated. Calibration tools.
* Barograph and thermograph from IMU sensor. Generate NMEA pressure and temperature data.
* Set system time from NMEA data
* Set time zone
* Set GPSD
* Select programs to run at startup