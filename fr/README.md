# Qu'est-ce qu'OpenPlotter?

![OpenPlotter logo](../en/openplotter500x300.png)

Certains achètent des bateaux quand d'autres les construisent. Pourquoi ne pas construire votre propre électronique ?
OpenPlotter est une combinaison de logiciels et de matériels utilisable comme aide à la navigation sur les petites et moyennes embarcations. C'est aussi une solution complète de domotique à destination de votre bateau. 

OpenPlotter fonctionne sur les ordinateurs a processeur ARM tel que le [Raspberry Pi](https://www.raspberrypi.org/) et est open-source, low-cost et consommant très peu. Sa conception est modulaire, vous pouvez donc n'installer et n'utiliser que ce qui vous est utile. Faites-le vous-même !

## Fonctionnalités

* **Traceur de cartes**. Grâce à  [OpenCPN](http://opencpn.org), logiciel de navigation Open Source réputé et ses nombreux plugins.
* **Prévisions météo**. Téléchargez et visualisez les fichiers Grib avec [zyGrib](http://www.zygrib.org).
* **Multiplexeur NMEA 0183**. Multiplexez et filtrez les données en provenance de sources réseau ou série illimitées. Envoyez ces données vers tout type de sortie.
* **Serveur Signal K (beta)**. OpenPlotter est prêt pour [Signal K](http://signalk.org/), le nouveau format gratuit, universel et open-source d'échange de données nautiques.
* **Moniteur NMEA**. Contrôlez les données échangées, diagnostiquez les éventuels conflits.
* **Point d'accès WiFi**. Partagez les données du bord (NMEA 0183, Signal K, bureau à distance, connexion internet) avec vos ordinateurs portables, smartphones, tablettes. Si une connexion internet est disponible, OpenPlotter pourra être votre point d'accès WIFI.
* **Ecran à distance**. Accédez à OpenPlotter de votre cockpit sur vos terminaux mobiles.
* **Headless**. Easy start without monitor.
* **Réception SDR-AIS**. Receive and decode AIS with cheap DVB-T dongles. Calibration tools Included.
* **Compas magnétique et gite**. Read magnetic heading and heel angle from an IMU sensor. Tilt compensated. Calibration tools Included.
* **Baromètre, Thermomètre and Hygromètre**. From pressure, temperature and humidity sensors. Save logs and display graphs to see trends.
* **Capteurs de température multiples**. Get data from coolant engine, exhaust, fridge, sea...
* **Capteurs spéciaux**. Detect opening doors/windows, tanks level, human body motion...
* **Déclinaison magnétique**. Calculate magnetic variation for date and position.
* **Cap vrai**. Calculate true heading from magnetic variation and magnetic heading.
* **Vent vrai**. Calculate true wind from apparent wind and either speed through water (speed log) or speed over ground (GPS).
* **Taux de virage**. Calculate the rate the ship is turning.
* **Monitoring à distance**. Publish data on Twitter or send it by email.
* **Actions pré-programmées**. Compare a custom value with any data flowing through your system and use it as a trigger to run multiple predefined actions.
* **Interrupteurs customs**. Connect external switches and link them with actions.
* **Composants customs**. Relays, LEDs, buzzers ...
* **Outils de mise à l'heure**. Set the system time from NMEA data and set the time zone easily.
* **Gestion des logiciels au démarrage**. Select some program parameters to automatically launch at start.

![OpenPlotter desktop](../en/openplotter.png)