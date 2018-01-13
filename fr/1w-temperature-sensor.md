# Capteur de température 1W

![](../en/DS18B20.png)

Il est possible de connecter, par ses câbles, le capteur 1W **DS18B20** à OpenPlotter. Ce capteur est étanche et supporte des températures élevées (~125°). En connectant plusieurs **DS18B20** en parallèle sur les mêmes broches, il est possible d'avoir la température du liquide de refroidissement du moteur, de l'échappement, de la câle moteur, du réfrigérateur, de l'eau de mer ...

>Cet article est disponible dans notre boutique[[1]](http://shop.sailoog.com)

## Câblage

Les noms des broches sont donnés par le diagramme suivant.

![](../en/RP2_Pinout.png)

Les capteurs de températures doivent être connectés aux broches **GPIO4** (soit GCLK), **GND** et **3.3V**. Certains capteurs peuvent posséder un quatrième fil qui n'a pas a être connecté. Il faut installer une résistance de rappel, comme indiqué sur le schéma ci-dessous. Il est possible d'installer plusieurs capteurs en parallèle, en n'utilisant qu'une seule résistance.

![](../en/DS18B20_sensors.png)

Si vous voulez changer de broche GPIO, éditez le fichier config.txt en tapant sur un terminal:

```sudo nano /boot/config.txt```

A la fin du fichier, vou devriez trouver une ligne telle que:

*dtoverlay=w1-gpio*

la remplacer par:

*dtoverlay=w1-gpio,gpiopin=x*

où x est la broche GPIO que vous souhaitez utiliser. Enregistrez et redémarrer.

## Configuration

Se reporter au chapitre [1W](/1w.md) pour configurer les capteurs **DS18B20**.

---

[1] http://shop.sailoog.com
