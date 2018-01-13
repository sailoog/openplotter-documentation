 # Qu'est-ce qu'OpenPlotter?

![OpenPlotter logo](../en/openplotter500x300.png)

Certains achètent un bateau, quand d’autres se le construisent. Si vous êtes de ceux là, pourquoi ne pas réaliser aussi l’électronique embarquée? OpenPlotter est un paquetage, matériel et logiciel, à utiliser comme aide à la navigation sur des petites ou moyennes unités. C’est aussi un système complet de domotique destiné aux bateaux. Il fonctionne sur ordinateur à processeur ARM tel que le Raspberry Pi[[1]](https://www.raspberrypi.org), est open-source, économique et peu consommateur. Sa conception est modulaire, il est donc possible de n’implémenter que ce qui est utile sur votre bateau. Faites-le vous-même!

## Fonctionnalités

* **OpenCPN**[[2]](http://opencpn.org), logiciel de navigation léger et robuste. Préparer des routes et suivre sa position.
* **zyGrib**[[3]](http://www.zygrib.org). Télécharger et visualiser des fichiers météo GRIB au format 1 et 2.
* **SDR-AIS**. Recevoir et décoder les signaux AIS via un dongle DVB-T. Outils de calibration inclus.
* **NMEA 0183**. Recevoir, filtrer, multiplexer et envoyer des données NMEA via le port série et les entrées/sorties du réseau.
* **NMEA 2000**. Se connecter à votre réseau NMEA 2000, via un adaptateur USB, pour recevoir et transmettre des données.
* **Signal K Server**[[4]](http://signalk.org).Convertir les données des capteurs en Signal K et échanger entre divers formats.
* **WiFi Access Point**. Partager les données NMEA et Signal K avec un portable, une tablette ou un smarphone.
* **Headless**. Accéder à OpenPlotter depuis le cockpit via vos appareils mobiles.
* **Dashboards**. Construire des tableaux de bord pour visualiser des données de navigation.
* **Compass**. Cap et gîte depuis un capteur IMU. Avec compensation d’inclinaison et auto calibration.
* **1W sensors**. Connecter de multiples capteurs : température, moteur, échappement, réfrigérateur, eau ...
* **I2C sensors**. Connecter des capteurs de température, pression, taux d’humidité ou des éclairages.
* **SPI sensors**. Mesurer la charge des batteries, le niveau des réservoirs ou n’importe quelle information d’un capteur analogique.
* **Digital inputs**. Connecter des interrupteurs, y compris spéciaux. Détecter fumée, ouverture de portes, mouvements ...
* **Digital outputs**. Activer des relais, des LED, des buzzers ...
* **Actions**. Utiliser date, heure ou n’importe quelle valeur de donnée manipulée par votre système comme déclencheur de multiples actions.
* **Share data**. Publier des informations sur votre bateau via Twitter ou envoyer des courriels / SMS automatiquement.
* **Remote Monitoring**. Recevoir ou envoyer des informations de votre bateau pendant que vous n’êtes pas à bord.
* **Open tools**. Utiliser les multiples outils inclus pour interargir avec le système et créer les vôtres.

![](../en/openplotter.jpg)

---
[1] https://www.raspberrypi.org [2] http://opencpn.org [3] http://www.zygrib.org [4] http://signalk.org
