# Optional
##Self powered USB Hub
![](hub.png)

If you are connecting devices which use more power than your Raspberry can manage, you will need a self powered USB Hub.

It would be a good idea to get a Hub with 5V input so that you could power it with the same source as your raspberry.

**Backpowering**

Backpowering occurs when USB Hubs do not provide a diode to stop the hub from powering against the host computer. This means that the hubs will power the Raspberry Pi through its USB cable input cable, without the need for a separate micro-USB power cable, and bypass the voltage protection. If you are using a hub that backfeeds to the Raspberry Pi and the hub experiences a power surge, your Raspberry Pi could potentially be damaged. In this case use "only data" cables or modify a normal USB cable cutting the Vcc pin.

##USB WIFI dongle

A Wi-Fi adapter will probably need more power than the Raspberry Pi USB port can provide, especially if there is a large distance from the Wi-Fi adapter to the Wi-Fi Access Point, or it is transferring large amounts of data. Therefore, you may need to plug the Wi-Fi adapter into a powered USB hub.

##USB GPS dongle
##USB RS422/RS232 converter dongle
##USB DVB-T dongle (AIS reception)
##Homemade AIS antenna
##IMU sensor
