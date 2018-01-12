# Capteur IMU

![](../en/imu.png)

Si vous n'avez pas de compas électronique embarqué, vous avez besoin d'un IMU.

Une centrale inertielle, ou IMU pour _Inertial Measurement Unit_, mesure et affiche la vitesse, l'orientation et les forces gravitationnelles, en utilisant la combinaison d'un accélérométre, d'un gyroscope et d'un magnétométre.

Connecter un IMU à OpenPlotter lui fournira le cap magnétique qui est utilisé pour calculer cap et vent vrai. Vous aurez aussi l'angle de barre.

>Cet article est disponible dans notre boutique[[1]](http://shop.sailoog.com)

## Capteurs IMU compatible

* InvenSense MPU-9150 mono chipset IMU.
* InvenSense MPU-6050 plus HMC5883 magnétométre sur bus aux MPU-6050 \(géré par le driver MPU-9150r\).
* InvenSense MPU-6050 gyros + accélérométres. (Considéré comme le MPU-9150 sans magnétométres).
* InvenSense MPU-9255 chipset IMU \(I2C et SPI\).
* STM LSM9DS0 mono chipset IMU.
* STM LSM9DS1 mono chipset IMU.
* L3GD20H + LSM303D \(optionellement avec le LPS25H\) comme utilisé sur le Pololu AltIMU-10 v4.
* L3GD20 + LSM303DLHC comme utilisé sur le Adafruit 9-dof \(ancienne version avec gyroscope GD20\) IMU.
* L3GD20H + LSM303DLHC \(optionellement avec le BMP180\) comme utilisé sur le nouveau Adafruit 10-dof IMU.
* Bosch BMX055 \(bien que le magnétométre soit actuellement expérimental\).
* Bosch BNO055 IMU avec onchip fusion. Note: no fiable avec RaspberryPi/Pi2 à cause de problématiques de stabilité d'horloge.

## Câblage

Les capteurs IMU doivent être connectés via l'interface I2C. Se référer au chapitre [Câblage des capteurs I2C](/wiring-i2c-sensors.md).

## Configuration

Voir le chapitre [Compas](/compass.md) pour configurer le capteur IMU.

---

[1] http://shop.sailoog.com
