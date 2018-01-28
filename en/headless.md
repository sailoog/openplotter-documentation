# Headless

You can use the RPI in headless mode after the NOOBS installation is done.

There are three ways to work headless.

1. Over a WiFi Access Point. See [WiFi AP](wifi-access-point.md) chapter.

2. You can connect to the RPI by an Ethernet cable and use the bonjour protocol or the bridged hotspot.

3. You can connect to the RPI by an USB cable to your tablet or smartphone and use the USB tethering feature. 

to 1\) After it has finished booting up, there should be a new WiFi network called _OpenPlotter_ available. Log onto this network using the password _my\_secret\_password_.

![](headless1.png)

to 3\) Selecting USB tethering

![](headless1c.png)

Finally, open your favourite VNC remote desktop client on your laptop, tablet or smartphone and make a new connection with the address/port combination: 
to 1\) and 2\) 
**10.10.10.1:5900**, or just the address **10.10.10.1** if you are using a RDP remote desktop client. 
to 3\) 
**192.168.42.100:5900**., or just the address **192.168.42.100** if you are using a RDP remote desktop client.


Connect and enjoy!

![](headless2.png)

See more information about tested remote desktop software in [Remote desktop](remote_desktop.md) chapter.

