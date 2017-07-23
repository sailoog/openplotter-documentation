# USB WiFi Stick


![](../en/wifi.png)

Du kannst OpenPlotter sowohl als Access Point zum Anschluß von anderen Tablets etc. benutzen, oder aber auch als Client an andere Access Points anschließen, etwa für einen Internet-Zugang. Das geht nicht gleichzeitig mit nur einem WiFi-Adapter. Um OpenPlotter gleichzeitig als Access Point und Client laufen zu lassen, werden bei einem Raspberry 3 ein zusätzlicher USB-WiFi-Stick benötigt, bei einem Raspberry 2 zwei USB-WiFi-Sticks.

Wenn OpenPlotter für den Internet-Zugang an einem Access Point angeschlossen ist und gleichzeitig selbst als Access Point eingestellt ist, kann der Internet-Zugang mit allen an OpenPlotter angeschlossenen Geräten geteilt werden. Dies kann sinnvoll etwa in Häfen sein, die nur eine Zugang zum Internet zulassen, aber an Bord meist mehrer Geräte Internet haben wollen. 

Ein guter WiFi-Stick kann mehr Strom benötigen als ein USB-Port des Raspberry Pi liefern kann, besonders dann, wenn der WiFi-Adapter eine große Entfernung zum Access Point überbrücken muss, oder wenn große Menge Daten über den Stick übertragen werden. Um dem Stick ausreichend mit Strom zu beliefern, sollte er an einem aktiven USB-Hub angeschlossen werden, d.h. einen USB-Hub mit eigener Stromversorgung.

Nicht alle WiFi-Sticks können als Access Point laufen, nur Sticks mit dem richtigen Chipset werden funktionieren. Wir empfehlen das **RTL8192CU/CUS** Chipset.

## Einstellungen

Siehe Kapitel [WiFI AP](/wifi-ap.md) zur Konfiguration von OpenPlotter als Client oder als Access Point.
