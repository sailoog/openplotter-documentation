# IMU sensor


![](../en/imu.png)

Hast Du keinen elektronischen Kompass an Bord, benötigst Du eine IMU.

Eine IMU (Inertial Measurement Unit, Inertiale Messeinheit) misst für die x-, y- und z-Achse Beschleunigungen und Drehraten und kann hieraus die Orientierung im Raum berechnen. In Kombination mit einem integrierten Magnetometer erhalten wir letztlich die Daten für den Magnetkompasskurs, und so wird die Berechnung von rechtweisendem Steuerkurs und wahrem Wind ermöglicht. Nebenher können  Krängung und Nickrate des Schiffes angezeigt werden.


##Unterstützte IMU Sensoren

* InvenSense MPU-9150 single chip IMU.
* InvenSense MPU-6050 plus HMC5883 Magnetometer auf dem Hilfsbus des MPU-6050 (verwaltet durch den MPU-9150 Treiber).
* InvenSense MPU-6050 Kreiselkompass und Beschleunigungsmesser. Gehandelt als MPU-9150 ohne Magnetometer.
* InvenSense MPU-9250 single chip IMU (I2C und SPI).
* STM LSM9DS0 single chip IMU.
* STM LSM9DS1 single chip IMU.
* L3GD20H + LSM303D (optional mit LPS25H), wie genutzt im Pololu AltIMU-10 v4.
* L3GD20 + LSM303DLHC, wie genutzt in der Adafruit 9-dof IMU (ältere Version mit GD20 gyro). (dof = degrees of freedem, Freiheitsgrade)
* L3GD20H + LSM303DLHC (optional mit BMP180), wie genutzt in der neuen Adafruit 10-dof IMU.
* Bosch BMX055 (obwohl mit Magnetometer-Unterstützung derzeit nur experimentell).
* Bosch BNO055 IMU mit onchip-Datenauswertung. Beachte: Wegen Timing-Problemen nicht stabil mit dem RaspberryPi/Pi2 einsetzbar.

## Anschluss

IMU Sensoren werden an das I2C-Interface angeschlossen. See Kapitel [Wiring I2C sensors](/wiring-i2c-sensors.md).
