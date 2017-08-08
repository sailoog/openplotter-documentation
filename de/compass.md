# Compass

Installiere den IMU-Sensor an der endgültigen Position auf dem Schiff, möglichst weit entfernt von Metallen und anderen magnetischen Störquellen, besonders von den Magneten von Lautsprechern. Nach dem Anschluss des IMU-Sensors soll er automatisch erkannt werden und im Tab _Kompass_ angezeigt werden.

Stelle die Aktualisierungsrate des Sensors ein und setze einen Haken bei mindestens einer drei möglichen Größe. Dann drücke auf _Kalibrierung_.

![](../en/compass.png)

Wenn das Boot vertaut im Hafen ruhig und so gerade wie möglich im Hafen liegt, wähle den _IMU_ Tab aus und drücke auf _Boat is level_. Nach ein paar Sekunden sollte die dreidimensionale Darstellung des Bootes ausgependelt dargestellt werden.

![](../en/imu_level.png)

Das Fenster _Kalibrierung_ wird noch nicht geschlossen, sondern der Tab _Kompass_ aufgerufen. Dann gehe segeln. Das System sammelt nun Daten vom IMU-Sensor. Wenn innerhalb von 2 Minuten die Richtung um mehr als 60 Grad geändert wird und die Daten gültig sind, wird der IMU-Sensor kalibriert. Eine blaue Kugel erscheint und die Wolke aus Punkten wird auf der roten Kugel dargestellt.

![](../en/imu_calibration.png)

Das System wird alle 2 Minuten neu kalibriert, solange mindestens eine der drei Größen des IMU-Sensors ausgewählt und ausreichend Daten gesammelt wurden. Alle 10 Minuten wird die Kalibrierung gespeichert, damit die Kalibrierung beim nächsten Programmaufruf gleich zur Verfügung steht. 
