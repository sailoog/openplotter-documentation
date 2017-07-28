# NMEA 0183 to USB converter

![](../en/rs422.png)

Wenn Du Navigationsgeräte oder andere Elektronik mit NME 0183-Ausgang an Bord hast (etwa für Wind, Echolot, Kompass...), kannst Du diese mit Hilfe eines USB-Konverters mit OpenPlotter verbinden. Ist der Konverter bidirektional, so ist es zudem möglich, Geräte mit NMEA 0183-Eingang anzusprechen. Dies wird z.B. für den Autopiloten benötigt.

Der NMEA 0183-Standard gibt die **RS422** Schnittstelle vor, jedoch findet man auch Geräte mit **RS232** Schnittstelle. Finde zunächst heraus, welchen Schnittstellen-Typ Du benötigst.
Du kannst die Schnittstelle im Allgemeinen so erkennen: Wenn Du die die Leitungen TX+ und TX- und/oder RX+ und RX- hast, ist es eine RS422-Schnittelle. Hast Du die Leitungen RX, TX und Masse(-) hast, ist es eine RS232-Schnittstelle.

## Einstellungen

Siehe Kapitel [NMEA 0183](/nmea-0183.md) zur Einstellung des NMEA 0183-USB Konverters.
