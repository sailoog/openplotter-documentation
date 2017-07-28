# NMEA 0183 to USB converter
---

**This chapter needs to be written/updated/translated**

http://forum.openmarine.net/forumdisplay.php?fid=16

---

![](../en/rs422.png)

Wenn Du Navigationsgeräte oder andere Elektronik mit NME 0183-Ausgang an Bord hast (etwa für Wind, Echolot, Kompass...), kannst Du diese mit Hilfe eines USB-Konverters mit OpenPlotter verbinden. Ist der Konverter bidirektional, so ist es zudem möglich, Geräte mit NMEA 0183-Eingang anzusprechen. Dies wird z.B. für den Autopiloten benötigt.

Der NMEA 0183-Standard gibt die **RS422** Schnittstelle vor, jedoch findet man auch Geräte mit **RS232** Schnittstelle. Finde zunächst heraus, welchen Schnittstellen-Typ Du benötigst.
In general, if you have a TX+ and a TX- and/or a RX- and RX+ you have a RS422 interface. If you ave a RX and a TX and a ground you have an RS232 interface.

## Einstellungen

Siehe Kapitel [NMEA 0183](/nmea-0183.md) zur Einstellung des NMEA 0183-USB Konverters.
