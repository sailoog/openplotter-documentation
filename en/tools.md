# Tools

In the tool menu are special modules.

The first three are:

---

* Set time zone

Opens a menu to choose a new time zone.

\(It is the same as utc+x or utc-x\)

---

* Set time from NMEA

The time from GPS \(RMC-sentence\) will be used to set the time of the RPI.

In future release it will read it from signalk \(then time can be taken not only from NMEA0183\).

\(If the RPI is connected to the internet it will get the time from a timeserver\)

---

* Set GPSD

Opens the configuration file of gpsd in editor nano.

For details of GPSD google is your friend

---

---

* [SDR receiver](sdr_ais.md)

SDR \(Software Defined Radio\) can be used to receive:

1. AIS

2. FM AM radio

3. VHF marine radio channel

4. weatherfax

5. 433/868 MHz remote controls or sensors

6. ...


Most cheap USB SDR can work from 30Mhz - 1.7GHz. So they can't receive navtex at 490kHz or 518kHz.

The antenna must be different for each frequence range to get good results.

---

* Calculate

This is used to calculate the true wind from apparent wind

![](/en/Calculate.jpg)

---

* NMEA 0183 generator

![](/en/nmea0183generator.jpg)

![](/en/nmea0183generatorForm.jpg)

---

* [NMEA 2000 generator](nmea-2k.md)

---

* [configureable tools](tools-defined.md)




