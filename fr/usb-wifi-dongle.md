#Dongle WiFi USB

![](../en/wifi.png)

OpenPlotter peut être configuré soit comme point d’accès, pour permettre à des appareils de se connecter, soit comme client pour se connecter lui-même à n’importe quel point d’accès. Faire les deux en même temps n’est pas possible avec un seul dispositif Wifi. Un dongle USB Wifi de plus sera nécessaire pour Raspberry 3 (deux, dans le cas d’un Raspberry 2 ne disposant pas de circuit Wifi interne).

Etre connecté à un point d’accès, en tant que client, pour établir une connexion Internet, et en même temps exécuter OpenPlotter en tant que point d’accès, permet de partager la connexion Internet avec tous les appareils connectés à OpenPlotter.

Un bon adaptateur WiFi aura probablement besoin de plus de puissance que ce que peut fournir un port USB du Raspberry, surtout si l’adaptateur est loin du point d’accès, ou si le volume transféré est important. Cependant, l’adaptateur WiFi peut être branché dans un hub USB alimenté.

Tous les adaptateurs WiFi ne fonctionnent pas en point d’accès. Seuls ceux avec le correct chipset conviendront. Le chipset recommandé est le **RTL8192CU/CUS**.


## Configuration

Se reporter au chapitre [WiFI AP](/wifi-ap.md) pour configurer OpenPlotter en tant que client ou point d’accès.
