# USB manager

Why is it important to manage the serial ports?

Linux does use standard port names. They are named by the connection time.

If you can guarantee that every time all usb adapter are connected and that there is no chance of malfunction on one device and you never put another device to the system, then you don’t need the USB manager.

Otherwise the names ttyUSBx are changeing \(for example the ais is on the autopilot port, the N2K Can-Bus is on the gps port…\). The multiplexer isn’t able to do his job any more.

Here the USB-ports can be setup manually.

![](/assets/screenshot.63.jpg)

Picture 1: already configured USB ports

select add to open a window of not configured serial ports.

![](/assets/screenshot.64.jpg)

Picture 2: adding a FTDI port

random name: the numbered port name which is given by linux

vendor product and serial: numbers and strings of the device

port: the usb-port position

![](/assets/screenshot.65.jpg)

Picture 3: USB port names of the raspberry pi

If you add a new serial port you can select remember by device or remember by port.

Remember by port can be used every time. See picture 3 it shows the usb port names of the raspberry pi.

But normally you want the system to get the right name independend of the port it is connected to.

You can do this if there is not a second device with identical information. In picture 1 you see for example an 4 port ftdi hub. It has a vendor and a product number and a serial string. But you have 4 times identical data. So you can't use remember by device. There are cheaper adapter which haven't got a serial number. If you have more than 1 of them you also can't use remember by device.

# Naming

The linux names ttyUSB0, ttyUSB4 don't have any information what is connected to the port so it's better to use a meaningful name.

The USB manager uses ttyOP\_xxxx.

Where xxxx belongs to personal decision. But we recommend to use

ttyOP\_N2K: for actisense ngt-1

ttyOP\_AP: for autopilot

ttyOP\_GP: for GPS

ttyOP\_II: for seatalk

ttyOP\_FIRM: for arduino with firmata

ttyOP\_MPXx: is used for multiplexers but it could be better to rename it to a meaningful name like AIS or PLOTTER.

There are other devices which doesn't send anything they 're only listening for sentences add a meanigful name to them.

To change a port name double click the line.

