# 1-Wire Temperatursensor


![](../en/DS18B20.png)

Zur Temperaturmessung kannst Du 1-Wire Temperatursensoren vom Typ **DS18B20** an OpenPlotter anschließen. Es gibt die Sensoren wie abgebildet in einer wasserdichten Ausführung (in einer Metallhülse), die Messung hoher Temperaturen bis 125°C ist mit sehr guter Genauigkeit möglich. In Form einer einer Bus-Leitung kann man mehrere DS18B20 parallel anschließen, sie haben zur Unterscheidung individuelle fest eingebrannte Adressen. Einsetzbar sind die Sensoren z.B. für Motorkühlung, Öltemperatur, Motorraum, Kühlschrank, Seewasser etc.

## Verdrahtung

Die Drahtenden werden gemäß der Abbildung unten angeschlossen.

![](../en/RP2_Pinout.png)

Die Temperatursensoren werden an die Pins **GPIO4** (auch GCLK genannt), **GND** und **3.3V** angeschlossen. Manche Sensoren haben einen vierten Draht, dieser wird nicht angeschlossen. Es ist erforderlich, einen Pull-Up Widerstand wie in der Abbildung (R1 = 4,7kOhm) anzuschliessen. Es wird nur ein Widerstand benötigt, auch bei Anschluss mehrerer DS18B20.

![](../en/DS18B20_sensors.png)

Wenn der GPIO-Pin GPIO04 geändert werden soll, ändere die Datei config.txt durch folgenden Aufruf auf Kommandoebene:

```sudo nano /boot/config.txt```

Am Ende der Datei steht diese Zeile:

*dtoverlay=w1-gpio*

Die Zeile wird so ersetzt:

*dtoverlay=w1-gpio,gpiopin=x*

bei X handelt es sich um den neu ausgewählten GPIO-Pin. Speichern mit CTRL-O, benden mit CTRL-X und neu starten (sudo reboot)
