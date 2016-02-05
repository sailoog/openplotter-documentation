# Headless

---

This chapter is under construction

---
In order to save money and power, you can use the system without monitor. Connecting your desktop computer, laptop, tablet or smartphone to OpenPlotter by remote desktop you will be able to access to the interface. To do this, we must convert openplotter into a WiFi hotspot to connect our devices.

Once we have created the SD card with OpenPlotter RPI, we have to insert it into any computer with any OS (Linux, MAC, Windows). The mounted device should be called *boot* and there should be a file called *config.txt*. Open this file in a text editor like notepad on windows, but not anything like MS Word which can save is as something which is not just plain text.

The top lines should look like this:

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
If you are going to connect to OpenPlotter by VNC remote desktop you have to remove the # chararter from words  *framebuffer_width* and *framebuffer_height* and set a size for your screen (800x600 by default). If you are going to connect to OpenPlotter by RDP remote desktop do not remove # chararters. See more information on Remote destop chapter.