# IMU sensor

![](imu.png)

If you don't have a electronic compass on board you will need an IMU.

An Inertial Measurement Unit, or IMU, measures and reports on velocity, orientation and gravitational forces, using a combination of an accelerometer, gyroscope, and a magnetometer.

Connecting an IMU to OpenPlotter will provide magnetic heading which is needed to calculate true heading and true wind. You will have heel angle data as well.

## Supported IMU sensors

* InvenSense MPU-9150 single chip IMU.
* InvenSense MPU-6050 plus HMC5883 magnetometer on MPU-6050's aux bus \(handled by the MPU-9150 driver\).
* InvenSense MPU-6050 gyros + acclerometers. Treated as MPU-9150 without magnetometers.
* InvenSense MPU-9255 single chip IMU \(I2C and SPI\).
* STM LSM9DS0 single chip IMU.
* STM LSM9DS1 single chip IMU.
* L3GD20H + LSM303D \(optionally with the LPS25H\) as used on the Pololu AltIMU-10 v4.
* L3GD20 + LSM303DLHC as used on the Adafruit 9-dof \(older version with GD20 gyro\) IMU.
* L3GD20H + LSM303DLHC \(optionally with BMP180\) as used on the new Adafruit 10-dof IMU.
* Bosch BMX055 \(although magnetometer support is experimental currently\).
* Bosch BNO055 IMU with onchip fusion. Note: will not work reliably with RaspberryPi/Pi2 due to clock-stretching issues.

## Wiring

IMU sensors have to be connected by I2C interface. See chapter [Wiring I2C sensors](/wiring-i2c-sensors.md).

## Settings

See [Compass](/compass.md) chapter to configure IMU sensors.
