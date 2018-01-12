# Le Stick CAN-USB

![](../en/can-usb-stick.png)

## Le projet

Le projet du Stick CAN-USB a été conduit pour analyser le flux de données d'un réseau N2K en envoyant et recevant des messages CAN. Le Stick est isolé électriquement pour éviter les dommages.

Le programme du micro-controlleur (MCU) a été revu pour travailler de concert avec le projet CANBOAT[[2]](https://github.com/canboat/canboat), lui-même utilisé par le projet Signal K[[3]](http://signalk.org). Ces deux paquetages sont utilisés par le projet OpenPlotter.

Le Stick CAN-USB fonctionne également avec le projet OpenSkipper[[4]](http://openskipper.org).

N'ont pas été testés:

* MacENC[[5]](http://macenc.com)
* PolarView NS[[6]](http://www.polarnavy.com)

Le Stick CAN-USB utilise les mêmes commandes que celles de l'interface Actisense-série de CANBOAT. Envoyer et recevoir des données depuis un réseau N2K peut être fait directement sous OpenPlotter.

Les nouveaux PGNs ne sont pas bloqués, puisqu'ils fonctionnent avec CANBOAT sur d'autres appareils. La vitesse de transmission peut être réglée plus haute que la vitesse du bus CAN bus. D'autre appareils, compatibles CANBOAT, ont une vitesse de transfert plus basse que le réseau N2K et peuvent devenir des goulots d'étranglement.

>Cet article est disponible dans notre boutique[[9]](http://shop.sailoog.com)

## Matériel

Le Stick CAN-USB V2 est basé sur un micro-controlleur **stm32** (MCU) connecté à un émetteur/récepteur CAN et un adaptateur USB-Série.

## Avertissement

le Stick CAN-USB est un projet de recherche sur la communication de données entre le bus CAN bus et un réseau N2K sur les bateaux.

Le programme est toujours en phase de développement et n'a pas été entièrement testé. Des disfonctionnements du Stick CAN-USB ou de tout appareil connecté sont possible à tout momment. Intervenir sur votre réseau N2K peut causer de dommages au appareils connectés.

**Ne pas se reposer sur les données fournies par le Stick CAN-USB et ne pas l'utiliser comme support principal à la navigation. Aucune responsabilité ne sera acceptée pour tout dommages, blessures de personnes ou disfonctionnements causés par cet appareil.**

Le Stick CAN-USB n'est pas certifié NMEA®.

L'utilisation du lecteur NMEA Actisense® pour le Stick CAN-USB n'est pas autorisée.

## N2K networks

![](../en/n2k_b.jpg)
_Auteur: Femnett/Maretron[[1]](https://commons.wikimedia.org/wiki/File:NMEA2000_Modified_motor_yacht.jpg), modifié par Sailoog, licence CC BY 2.5._

![](../en/n2k_a.jpg)  

_Exemple d'un petit réseau N2K._

Les réseaux N2K sont décrit dans Wikipedia[[7]](https://en.wikipedia.org/wiki/NMEA_2000).
La colonne vertébrale (backbone) commence et finit par un bouchon de terminaison 120Ω (deux résistances peuvent travailler en parallèle, donc la résistance est de 120Ω/2=60Ω). S'il y a un connection rompue dans le backbone vous ne pourrez mesurer que 120Ω ou rien mais pas  60Ω. C'est un moyen très facile de vérifier le bus.

![](../en/resistor_conn.jpg)  
_Bouchon de terminaison mâle 120Ω_

Une branche alimentant les appareils ne peut faire plus de 6m. La longueur du backbone est limitée à 100m.

Le Stick CAN-USB est isolé électriquement, les appareils et votre ordinateur sont donc protégés même s'ils sont alimentés par d'autres sources que votre réseau N2K.

## Connexion

Pour connecter le Stick CAN-USB au réseau, vous avez besoin d'un connecteur en T libre sur votre backbone et d'une branche. La branche doit avoir d'un coté un connecteur mâle M12 5 broches et de l'autre 5 fils (bien que seuls 2 soient utilisés). Le connecteur HIRSCHMANN ELST 5012 PG7 a une terminaison visée.

![](../en/t-conn.jpg)  
_Connecteur en T_

![](../en/m12_conn.jpg)  
_Branche coté connecteur mâle M12 5 broches._

![](../en/micro_cable.jpg)  
_Branche coté fils_

![](../en/can_usb_connect.jpg)

* Dévisser les vis de l'embout vert du Stick.
* Connecter le fil bleu de la broche 5 de la branche (broche du milieu) au CANL sur l'embout vert du Stick.
* Connecter le fil blanc de la broche 4 de la branche au CANH sur l'embout vert du Stick.
* Ouvrir l'interrupteur principal, pour être sûr qu'il n'y a plus du courant sur le réseau.
* Connecter la branche au connecteur en T libre sur votre backbone.
* Utiliser un volmétre pour mesurer la résistance entre CANH et CANL (sur les vis). Elle doit être d'environ 60Ω.
* Connecter l'embout vert au Stick CAN-USB.
* Vérifier à nouveau les 60Ω entre CANH et CANL.
* Il reste trois fils sur la branche qui doivent être isolés.
* Alumer l'alimentation principale.
* Alumer les instruments.

Pour configurer votre Stick CAN-USB, se référer au chapitre [N2K](n2k.md). Sous Windows utiliser OpenSkipper.

## LED

La LED du Stick CAN-USB est éteinte pendant 10" durant la séquence de démarrage puis:

- Allumée en permanence, si non connecté au réseau.
- Allumée pendant 1", si connecté au réseau.
- Eteinte, s'il n'y a pas de flux de données.
- Scintillante si un flux de données transite.

## Support

Si vous avez besoin de support, ou pour toute suggestion, vous pouvez publier vos questions sur le forum OpenMarine[[8]](http://forum.openmarine.net/forumdisplay.php?fid=11).

---

[1] https://commons.wikimedia.org/wiki/File:NMEA2000_Modified_motor_yacht.jpg [2] https://github.com/canboat/canboat [3] http://signalk.org [4] http://openskipper.org [5] http://macenc.com [6] http://www.polarnavy.com [7] https://en.wikipedia.org/wiki/NMEA_2000 [8] http://forum.openmarine.net/forumdisplay.php?fid=11 [9] http://shop.sailoog.com


