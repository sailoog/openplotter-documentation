# Getting started

First of all you have to put together all the [required parts](what_do_you_need.md). If you have trouble with some aspect, try to find help on the [Raspberry Pi official page](https://www.raspberrypi.org/help/).

Second you have to run the software on your ARM computer and here you have two options, either buy our plug and play SD card or download and install the software on an SD card.

---

**Buy an 8 GB SD card with OpenPlotter RPI ready to run.**

[http:\/\/www.sailoog.com\/shop-category\/openplotter](http://www.sailoog.com/shop-category/openplotter)

---

## Installing OpenPlotter RPI on an SD card

Download the last noobs version of **OpenPlotter RPI** from

[http:\/\/sailoog.com\/blog-categories\/openplotter-rpi](http://sailoog.com/blog-categories/openplotter-rpi)

It is a compressed file ca. 1GB so it will take a while.

Once the download is completed we have to unzip it and copy all files from the noobs folder onto a micro SD FAT32 formated card minimum 8 GB.

In the noobs menu select OpenPlotter and click install. It takes several minutes to format and install the system.

1. On the first start you will be warned to type in a new password.

2. AutoSetup pops up.[/auto-setup-usb-ports.md](/auto-setup-usb-ports.md)

3. The monitor will be auto detected. \(The right settings for 800x480 monitor will work on next boot\)


First boot

If you want to build a headless system see the next chapter [Headless](headless.md) before reading further.

Once we have created the SD card with OpenPlotter RPI, we will insert it into our Raspberry Pi.

![](boot1.png)

Connect power to the RPI. We wait for the noobs menu.

In the noobs menu we select openplotter and click install. It takes several minutes to format and install the system.

If you bought our SD card you just turn on the system and start.

1. On the first start you will be warned to type in a new password.

2. [AutoSetup](/auto-setup-usb-ports.md) pops up.

3. The monitor will be auto detected. \(The right settings for 800x480 monitor will work on next boot\)


Go to _Menu_ &gt; _Preferences_ and select _Raspberry Pi Configuration_.

![](RPIsetup1.jpg)

A window will open and it's a good idea to change the Password to make OpenPlotter more secure. Click on _Change Password_ \(default password: raspberry\).

![](RPIsetup3.jpg)

## Setting language and country

You need to set your system localisation, click on the _Localisation_ tab and then on _Set Locale_, _Set Timezone, _ _Set Keyboard, Set WiFi Country_ buttons.

![](RPIsetup2.jpg)

To configure openplotter we start with setting up the usb adapter [Auto Setup USB ports](auto-setup-usb-ports.md).

# Security

Because of security reasons **ssh is disabled by default** and can be activated under Interfaces.

Then we can use:

on windows system PuTTY and WinSCP

on linux system putty and nautilus

to exchange files and get a remote terminal.

**Keep it disabled if you don't need it!**