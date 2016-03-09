# BUREAU A DISTANCE (Headless)

Pour économiser énergie électrique (et argent), vous pouvez utiliser OpenPlotter sans écran dédié: un terminal mobile connecté en WIFI vous permettra d'accéder à l'interface. A cette fin, vous utiliserez le mode point d'accès WIFI d'OpenPlotter:

Une fois la carte SD OpenPlotter créée, insérez-la dans un ordinateur (linux, MAC ou Windows). La carte apparaîtra sous le nom "*boot*", et vous y trouverez un fichier nommé *config.txt*. 

Ouvrez ce fichier avec votre éditeur de texte favori (Notepad, Notepad++) à l'exception des traitements de textes tels que MSWords (qui ne sauvegardent pas le texte sous sa forme "brute").
 
Voici les premières lignes de ce fichier:

```
[OPENPLOTTER]

#HEADLESS

#uncomment to force screen resolution (only VNC remote desktop)
#framebuffer_width=800
#framebuffer_height=600

#uncomment to set WiFi access point
#device=wlan0
#ssid=OpenPlotter
#pass=12345678

[RASPBIAN]
...
```
- Pour un accès distant à OpenPlotter avec VNC remote desktop:

Retirez le caractère **#** devant ***framebuffer_width*** et ***framebuffer_height***, puis spécifiez la taille de l'écran (800x600 par défaut).

Pour un accès avec RDP remote desktop, vous n'avez pas de modification a faire: vous ajusterez la taille de l'affichage dans logiciel RDP. 

Vous trouverez plus de détails dans le chapitre [Remote desktop](remote_desktop.md).

- Pour créer le point d'accès WIFI:

Retirez le caractère **#** précédant ***device***, ***ssid*** and ***pass***. 
Si une seule clé WIFI est présente sur votre Rapberry Pi, la valeur de *device* devra être *wlan0* mais si plusieurs clé wifi sont en place, vous pourrez choisir entre  *wlan0*, *wlan1*, etc... 

*ssid* sera le nom de votre réseau WIFI. Si vous choisissez de modifier ce nom (par defaut: "OpenPlotter"), n'utilisez pas plus de 32 caractères.

*pass* sera le mot de passe de votre réseau WIFI. remplacez "12345678" par le mdp de votre choix (min. 8 caractères)

Après édition, votre fichier doit ressembler à cela:

```
[OPENPLOTTER]

#HEADLESS

#uncomment to force screen resolution (only VNC remote desktop)
framebuffer_width=800
framebuffer_height=480

#uncomment to set WiFi access point
device=wlan0
ssid=my_boat_network
pass=my_secret_password

[RASPBIAN]
...
```

Save and eject the SD card, then insert it into the Raspberry Pi. Make sure the WiFi dongle is also inserted and power up the Pi.

After it has finished booting up, there should be a new WiFi network called *my_boat_network* available. Log onto this network using the password *my_secret_password*.

![](headless1.png)

Finally, open your favourite VNC remote desktop client on your laptop, tablet or smartphone and make a new connection with the address/port combination: **10.10.10.1:5900**, or just the address **10.10.10.1** if you are using a RDP remote desktop client.

Connect and enjoy!

![](headless2.png)

See more information about tested remote desktop software in [Remote desktop](remote_desktop.md) chapter.

If this is your first boot, go to [Getting Started](getting_started.md) chapter and follow the steps.

