# Getting started

First of all you have to put together at least all the [required hardware parts](what_do_you_need.md).

Then, you have to run the software on your Raspberry. **OpenPlotter RPI** is a modified version of [Raspbian](https://www.raspbian.org/), the official operating system for the Raspberry Pi. It contains all you need. OpenPlotter RPI is open-source and free.

Here you have two options, either buy our plug and play SD card or download and install the software on an SD card.

---

**8GB/16GB SD card with OpenPlotter RPI ready to run.**  
\(waiting for v0.9.xbeta to be released\)  
[shop.sailoog.com](http://shop.sailoog.com).

---

## Installing OpenPlotter RPI on an SD card

Any micro-SD-compatible card will work on your Raspberry. However, there are some guidelines that should be followed.

A minimum of 8GB is required but 16GB is recommended.

The card class determines the sustained write speed for the card; a class 4 card will be able to write at 4MB/s, whereas a class 10 should be able to attain 10 MB/s. However it should be noted that this does not mean a class 10 card will outperform a class 4 card for general usage, because often this write speed is achieved at the cost of read speed and increased seek times.

To begin with, it's always a good idea to make sure you have formatted your SD card. You'll need to make sure your computer has a built-in SD card reader, or you can use a USB SD card reader.

Visit the [SD Association’s website](http://www.sdcard.org/\) and download [SD Formatter 4.0]\(https://www.sdcard.org/downloads/formatter_4/index.html) for either Windows or Mac.

Follow the instructions to install the software.

Insert your SD card into the computer or laptop’s SD card reader and make a note of the drive letter allocated to it, e.g. F:/.

In SD Formatter, select the drive letter for your SD card and format it.

![](SD-Formatter.jpg)

Download the latest NOOBS installer version of **OpenPlotter RPI** from

[www.sailoog.com/en/blog-categories/openplotter-rpi](http://www.sailoog.com/en/blog-categories/openplotter-rpi)

It is a compressed file of about 1GB so it will take a while.

Extract the files from the zip.

Once your SD card has been formatted, drag all the files in the extracted NOOBS folder and drop them onto the SD card drive.

The necessary files will then be transferred to your SD card.

When this process has finished, safely remove the SD card and insert it into your Raspberry Pi.

![](boot1.png)

## First boot

Connect power to the Raspberry Pi.

OpenPlotter NOOBS installer will make a silent install, this means that you do not have to do anything. It will take several minutes to format partitions and install the system.

**If you are on an headless system you have to wait until a WiFi network named "OpenPlotter" apears on your client computer. The default password is "12345678", please change this as soon as possible on WiFi AP tab. For more information see **[**Headless**](/headless.md)** chapter.**

Once the OpenPlotter NOOBS installer has installed OpenPlotter RPI, it will start directly every time we connect the Raspberry Pi.

## Recovery system

If our system gets damaged or unstable, we can install OpenPlotter RPI again pressing the Shift key when we see this symbol at startup:

![](recovery.png)

**We will lose all data, manually installed programs and settings after installation.**

## Settings

The nativ monitor resolution for 800x480 monitors will be auto detected. The right settings for it will work on the next boot! If we have such a monitor. We do a restart.

Auto Setup window will pop up to help us to configure the USB connected devices. We can skip or close it. It will appear on every boot until we uncheck setup autostart on every boot. For more information see [Auto Setup USB Ports](/auto-setup-usb-ports.md) chapter.

Go to Menu > Preferences and select _Raspberry Pi Configuration_.

![](RPIsetup1.jpg)

A window will open where you can personalise your system. It is a good idea to change the Password to make OpenPlotter more secure. Click on _Change Password_ (default password: raspberry).

![](RPIsetup3.jpg)

If you need to set your system localisation, click on the _Localisation_ tab and then on _Set Locale_ (language), _Set Timezone, _ _Set Keyboard, Set WiFi Country_ buttons.

![](RPIsetup2.jpg)



