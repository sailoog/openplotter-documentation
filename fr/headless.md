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
If you are going to connect to OpenPlotter by VNC remote desktop, you have to remove the # character from words  ***framebuffer_width*** and ***framebuffer_height*** and set the screen size (800x600 by default). 

If you are going to connect to OpenPlotter by RDP remote desktop, you do not have to remove the # characters from words *framebuffer_width* and *framebuffer_height*, you will set the screen size from RDP software. See more information in [Remote desktop](remote_desktop.md) chapter.

To create the WiFi hotspot you have to remove the # character from words ***device***, ***ssid*** and ***pass***. 

If only one WiFi dongle is connected, the *device* value should always be *wlan0* but if more than one is connected, the *device* value could be *wlan0*, *wlan1* ...

*ssid* will be the name of your WiFi network. Use any character but a maximun of 32.

*pass* will be the password of your WiFi network. Use any character but a minimum of 8.

After changes, the top lines should look like this:

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

