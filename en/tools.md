# Tools

In the tool menu are special modules.

![](toolsMenu.png)

The first three are:

---

* Set time zone

Opens a menu to choose a new time zone.

\(It is the same as utc+x or utc-x\)

---

* Set time from NMEA

The time from GPS \(RMC-sentence\) will be used to set the time of the RPI.

In future release it will read it from SignalK \(then time can be taken not only from NMEA0183\).

\(If the RPI is connected to the internet it will get the time from a timeserver\)

---

* Set GPSD

Opens the configuration file of GPSD in editor nano.

For details of GPSD google is your friend

---

---

* [SDR receiver](sdr-receiver.md)

SDR \(Software Defined Radio\) can be used to receive:

1. AIS

2. FM AM radio

3. VHF marine radio channel

4. weatherfax

5. 433/868 MHz remote controls or sensors

6. ...


Most cheap USB SDR can work from 30 Mhz - 1.7 GHz. So they can't receive navtex at 490 kHz or 518 kHz.

The antenna must be different for each frequency range to get good results.

---

* Calculate

This is used to calculate the true wind from apparent wind

![](Calculate.jpg)

---

* NMEA 0183 generator

This tool allows you to create your own NMEA0183 sentences. You can select which SignalK value you want to take.

SignalK values are based on SI units (m,m²,m³,m/s,m³/s,J,rad,K,Pa,A,V,Hz,W)
NMEA 0183 uses different units.
That means you have to subtract for example 273.15 from a temperature value and to get radiant to degree you have to multiply by 57.29578.

![](nmea0183generator.jpg)

![](nmea0183generatorForm.jpg)

To activate the changed configuration go to _SignalK_ tab and click restart.

To check the result of the changes go to _NMEA 0183_ tab -click on system -click on diagnostic.

---

* [NMEA 2000 generator](nmea-2k.md)

---

* [configureable tools](tools-defined.md)




