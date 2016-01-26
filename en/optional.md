# Optional

---

This chapter is under construction

---



##USB NMEA 0183 converter dongle
![](rs422.png)

If you have sensors and electronics with NMEA 0183 outputs on board (depth, wind, heading...) you will need an USB converter to connect it to OpenPlotter. Additionally, you will be able to talk to electronics with NMEA 0183 inputs (autopilot).

The NMEA 0183 hardware standard uses RS422 connectors but you may find some devices with RS232 as well. 

####Buy a tested USB NMEA 0183 bi-directional converter.

Select your right connector.

http://www.sailoog.com/shop-category/openplotter

##USB DVB-T dongle (AIS reception)
![](sdr.png)

DVB-T dongles based on the Realtek RTL2832U chip can be used as a cheap one channel AIS receptors.

A DVB-T dongle will need more power than the Raspberry Pi USB port can provide. You need to plug the dongle into a powered USB hub.

####Antenna

Any VHF antenna will work right. Some homemade antennas:

http://sdrformariners.blogspot.com.es/p/blog-page.html

http://nmearouter.com/docs/ais/aerial.html

https://www.youtube.com/watch?v=SdEglNHyHB4

####Buy a tested USB DVB-T/RTL-SDR dongle.

With the RTL2832U+R820T2 chipset.

http://www.sailoog.com/shop-category/openplotter

##IMU sensor
![](imu.png)

If you don't have a electronic compass on board you will need an IMU.

An Inertial Measurement Unit, or IMU, measures and reports on velocity, orientation and gravitational forces, using a combination of an accelerometer, gyroscope, and a magnetometer.

Connecting an IMU to OpenPlotter will provide magnetic heading which is needed to calculate true heading and true wind.

####Supported IMU sensors

* InvenSense MPU-9150 single chip IMU.
* InvenSense MPU-6050 plus HMC5883 magnetometer on MPU-6050's aux bus (handled by the MPU-9150 driver).
* InvenSense MPU-6050 gyros + acclerometers. Treated as MPU-9150 without magnetometers.
* InvenSense MPU-9250 single chip IMU (I2C and SPI).
* STM LSM9DS0 single chip IMU.
* STM LSM9DS1 single chip IMU.
* L3GD20H + LSM303D (optionally with the LPS25H) as used on the Pololu AltIMU-10 v4.
* L3GD20 + LSM303DLHC as used on the Adafruit 9-dof (older version with GD20 gyro) IMU.
* L3GD20H + LSM303DLHC (optionally with BMP180) as used on the new Adafruit 10-dof IMU.
* Bosch BMX055 (although magnetometer support is experimental currently).
* Bosch BNO055 IMU with onchip fusion. Note: will not work reliably with RaspberryPi/Pi2 due to clock-stretching issues.


##Pressure/Temperature sensor
![](bmp180.png)

Often, pressure and temperature sensors are on the same board. You will get graphs to monitor weather.

####Supported pressure/temperature sensors
* BMP180
* LPS25H
* MS5611
* MS5637
