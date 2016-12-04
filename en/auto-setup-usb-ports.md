# Auto Setup USB ports

On Linux serial USB ports are numbered in the sequence they are detected.

This could work some times. But it isn't reliable. If of any reason you loose a contact between the raspberry pi and an USB-serial port adapter. It could be that the entire configuration doesn't work anymore!

A more reliable way is, to give every serial port a name.

This is the reason why auto setup pop up on a fresh system.

# Start tty auto setup

* all your devices should be connected to the internal \/ external USB-Hub \(inclusive USB-gps-dongle and special CAN-BUS to USB adapter like actisense NGT-1 or !!link!!\)

* turn on all your NMEA 0183 devices


![](/en/autosetup_popup.jpg)

* If setup autostart on every boot is checked uncheck it

* start the setup process by the setup buttom.


The tty auto setup can be started manually by Tools-&gt;Auto Setup Start

Auto setup is sometimes able to find

* NMEA 0183 ports

It auto detects the baud rate and checks if there are only NMEA 0183 sentences of one device-ID.

example1: $APxxx

* It will select the port name ttyOP\_AP

example2: $GPxxx

* It will select the port name ttyOP\_GP

If there are more device-IDs it will select ttyOP\_MPX1, next tty\_MPX2,...

If it detects an openplotter compatible CAN-USB adapter it selects ttyOP\_N2K

To check if everything is done go to [USB manager.](usb-manager.md)

