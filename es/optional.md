# Opcional
##Hub USB auto-alimentado
![](hub.png)

Si estás conectando dispositivos que usan más corriente de la que la Raspberry puede servir, necesitas un Hub o concentrador USB auto-alimentado.

Lo ideal es usar un Hub alimentado a 5V así podrás usar la misma fuente con la que alimentas la Raspberry.

####Compra un Hub USB comprobado.
Barato Hub USB 2.0 alimentado a 5V.

http://www.sailoog.com/shop-category/openplotter

##Dispositivo WiFi USB
![](wifi.png)

Si quieres conectarte a Internet o conectar tus dispositivos móviles a OpenPlotter (punto de acceso) necesitarás un dispositivo WiFi USB.

Este dispositivo probablemente necesitará bastante corriente, especialmente si hay una gran distancia entre equipos o se están transfiriendo grandes volúmenes de datos. Debido a esto, posiblemente necesitarás conectar el dispositivo WiFi a un Hub USB auto-alimentado.

####Punto de acceso WiFi

Para compartir datos con otros equipos de abordo vía WiFi o usar un escritorio remoto, tienes que configurar OpenPlotter como punto de acceso y conectar estos equipos al mismo. Sin embargo no todos los dispositivos WiFi USB pueden funcionar como punto de acceso, solo los dispositivos con el chipset **RTL8192CU** o **RTL8188CUS** funcionarán sin problemas en la Raspberry.

##Dispositivo GPS USB
![](gps.png)

If you don't have any GPS on board or you want an extra positioning device, this is the cheapest way.

Connecting an USB GPS dongle to OpenPlotter will provide accurate position, date/time and speed/course over ground.

####Buy a tested GPS/GLONASS USB dongle.

Low-power, GPS/GLONASS compatible, NMEA-0183 output.

http://www.sailoog.com/shop-category/openplotter

##USB RS422/RS232 converter dongle
![](rs422.png)

If you have sensors and electronics with NMEA-0183 outputs on board you will need an USB converter to connect it to OpenPlotter. Additionally, you will be able to talk to electronics with NMEA-0183 inputs.

The NMEA-0183 hardware standard uses RS422 connectors but you may find some devices with RS232 as well. 

####Buy a tested USB RS422/RS232 bi-directional converter.

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

An Inertial Measurement Unit, or IMU, measures and reports on velocity, orientation and gravitational forces, using a combination of an accelerometer, gyroscope, and a magnetometer. Some IMUs are also fitted with a barometric sensor and a temperature sensor.

Connecting an IMU to OpenPlotter will provide magnetic heading which is needed to calculate true heading and true wind. Besides, if barometric and temperature sensors are included, you will get graphs to monitor the weather.

####Supported IMUs

**Accelerometer/Gyroscope/Magnetometer sensors 
**
* InvenSense MPU-9150 single chip IMU.
* InvenSense MPU-6050 plus HMC5883 magnetometer on MPU-6050's aux bus (handled by the MPU-9150 driver).
* InvenSense MPU-6050 gyros + acclerometers. Treated as MPU-9150 without magnetometers.
* InvenSense MPU-9250 single chip IMU (I2C and SPI)
* STM LSM9DS0 single chip IMU
* L3GD20H + LSM303D (optionally with the LPS25H) as used on the Pololu AltIMU-10 v4.
* L3GD20 + LSM303DLHC as used on the Adafruit 9-dof (older version with GD20 gyro) IMU. 
* L3GD20H + LSM303DLHC (optionally with BMP180) as used on the new Adafruit 10-dof IMU.
* Bosch BMX055 (although magnetometer support is experimental currently).

**Pressure/Temperature sensors**
* BMP180
* LPS25H
* MS5611
* MS5637
