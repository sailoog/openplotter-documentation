# USB WiFi dongle

![](wifi.png)

You will need an USB WiFi dongle if you are using a Raspberry Pi 2 model (no built-in WiFi) and you want to run OpenPlotter as an access point or connect to a router. If you are using a Raspberry 3 model (built-in WiFi) you will need an extra WiFi device to run OpenPlotter as an access point and conect to a router at the same time.

A good WiFi adapter will probably need more power than the Raspberry Pi USB port can provide, especially if there is a large distance from the WiFi adapter to the WiFi Access Point, or it is transferring large amounts of data. Therefore, you may need to plug the WiFi adapter into a powered USB hub.

To share data with on board devices by WiFi you have to set OpenPlotter as an access point and connect devices to it. However not all WiFi dongles can function as an access point, only devices with the correct chipset will work. We recommend **RTL8192CU/CUS** chipset.
