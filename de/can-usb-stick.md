# CAN-USB Stick

![](../en/can-usb-stick.png)

## Projekt

Die Analyse des Datenstroms in einem N2K-Netzwerk (CAN-Bus), das Empfangen und Senden von CAN-Bus-Telegrammen, war der Auslöser für das Projekt CAN-USB Stick. Zum Schutz vor Schäden wurde eine elektrische Isolierung vorgesehen.

Das Programm des Mikrocontrollers im Stick (MCU) wurde neu erstellt, um mit dem Projekt CANBOAT[[2]](https://github.com/canboat/canboat) zu funktionieren. CANBOAT wird vom Projekt Signal K[[3]](http://signalk.org) genutzt. Beide Pakete sind im Projekt OpenPlotter enthalten.

Der CAN-USB Stick funktioniert auch mit dem Projekt OpenSkipper[[4]](http://openskipper.org).

Nicht getestet:

* MacENC[[5]](http://macenc.com)
* PolarView NS[[6]](http://www.polarnavy.com)

Der Stick nutzt die Kommandos des Programms CANBOAT actisense-serial. Weiterhin geschieht das Senden und Empfangen von N2K-Daten direkt aus OpenPlotter heraus.

Neue PGN's werden nicht blockiert, sie können mit anderen Geräten, die auch mit CANBOAT zusammenarbeiten, verarbeitet werden. Die Übertragungsrate kann schneller eingestellt werden als die des CAN-Bus. Andere Geräte, die CANBOAT nutzen, arbeiten vielleicht mit einer niedrigeren Übertragungsgeschwindigkeit als das N2K-Netzwerk und können eventuell überfordert werden.

## Hardware

Der CAN-USB Stick V2 basiert auf einem stm32-Mikrocontroller (MCU), welcher mit einem isolierten CAN-Transceiver und einem USB-Seriell-Konverter verbunden ist.

## Warnung / Haftungsausschluss

CAN-USB Stick ist ein Forschungsprojekt für die Datenkommunikation auf dem CAN-Bus bzw. in einem N2K-Netzwerk.

Das Programm ist noch in der Entwicklung und noch nicht vollständig getestet. Fehlfunktionen des CAN-Bus oder in irgendeinem anderen angeschlossenen Gerät sind jederzeit möglich. Die Manipulierung des N2K-Netzwerkes kann Schäden an den angeschlossenen Geräten verursachen.

Verlassen Sie sich nicht auf Daten von diesem Gerät und verwenden Sie es nicht als primäre Quelle für die Navigation. Für Schäden, Verletzungen oder durch dieses Gerät verursachte Störungen kann keine Haftung übernommen werden.

Der CAN-USB Stick ist nicht von NMEA® zertifiziert.

Es ist nicht erlaubt,das Actisense® NMEA Reader Programm mit dem CAN-USB Stick zu nutzen.

## N2K-Netzwerke

![](../en/n2k_b.jpg)

Autor: Femnett/Maretron[[1]](https://commons.wikimedia.org/wiki/File:NMEA2000_Modified_motor_yacht.jpg), geändert von Sailoog, CC BY 2.5 Lizenz.

![](../en/n2k_a.jpg)  

Beispiel eines kleinen N2K-Netzwerkes.

Das N2K-Netzwerk ist auf Wikipedia[[7]](https://en.wikipedia.org/wiki/NMEA_2000) beschrieben. Das Backbone (oder die Stammleitung) beginnt mit einem 120Ω Terminator und endet auch mit einem 120Ω Terminator. Zwei Widerstände arbeiten somit parallel, wodurch sich der effektive Gesamtwiderstand von 120Ω/2 = 60Ω ergibt. Wenn es eine Unterbrechung auf der Stammleitung gibt, kann man 120Ω messen, und nicht 60Ω. Dies ist ein einfacher Weg den Bus zu prüfen.

![](../en/resistor_conn.jpg)  

M12 120Ω Terminator (Ausführung als Stecker)

Die Stichleitung zu den Geräten soll nicht länger als 6m sein. Die Stammleitung darf 100m lang sein.

Der CAN-USB Stick ist isoliert, um die angeschlossenen Geräte und den Computer zu schützen, falls sie von einer anderen Stromquelle als das N2K-Netzwerk versorgt werden.

## Anschluss

Um den CAN-USB Stick an das N2K-Netzwerk anzuschließen, wird ein freies T-Stück auf der Stammleitung sowie eine Stichleitung benötigt. Die Stichleitung soll einen M12 5-Pin Stecker auf der einen Seite haben und auf der anderen Seite 5 freie Adern auf der anderen Seite haben. Von den 5 Adern werden nur 2 benötigt. Der HIRSCHMANN ELST 5012 PG7 Stecker hat einen Block mit Schraubanschlüssen.

![](../en/t-conn.jpg)  
T-Stück


![](../en/m12_conn.jpg)  
Stichleitung auf der Seite mit M12 5-Pin Stecker


![](../en/micro_cable.jpg)  
Stichleitung auf der Seite mit den fünf freien Adern


![](../en/can_usb_connect.jpg)

* Ziehe den grünen Block mit den Schraubanschlüssen aus dem Stick.
* Schließe von der Stichleitung die blaue Ader (Pin 5, der Pin in der Mitte) an den Anschluss CANL an.
* Schließe von der Stichleitung die weisse Ader (Pin 4) an den Anschluss CANH an.
* Schalte den Hauptschalter aus um sicher zu sein, dass auf dem N2K-Netzwerk keine Spannung ist.
* Schließe die Stichleitung an das freie T-Stück an.
* Benutze ein Multimeter und messe den Widerstand zwischen den Kontakten CANH und CANL. Der Widerstand soll ca. 60 Ohm  betragen.
* Stecke den grünen Anschlussblock wieder in den Stick.
* Messe nochmals den Widerstand zwischen CANH and CANL, er soll immer noch ca. 60 Ohm betragen.
* An der Stichleitung bleiben nun noch drei Leitungen unbenutzt, diese müssen isoliert werden.
* Schalte den Hauptschalter wieder ein.
* Schalte die Instrumente ein.

Um den CAN-USB Stick einzustellen, lies das Kapitel [N2K](n2k.md). Unter Windows nutze OpenSkipper.

## LED

Die LED am CAN-USB Stick bleibt für 10 Sekunden **AUS** während der Startsequenz, dann:

- Dauerhaft **AN** wenn der Stick nicht an das N2K-Netzwerk angeschlossen ist.
- **AN** für eine Sekunde wenn der Stick an das N2K-Netzwerk angeschlossen ist.
- Dauerhaft **AUS** wenn keine Daten eingehen.
- **BLINKEN** wenn Daten eingehen.

## Unterstützung

Wenn Du Unterstützung benötigst oder Vorschläge machen möchtest, kannst Du Deine Fragen auf dem Forum von OpenMarine[[8]](http://forum.openmarine.net/forumdisplay.php?fid=11) einstellen.

---

[1] https://commons.wikimedia.org/wiki/File:NMEA2000_Modified_motor_yacht.jpg [2] https://github.com/canboat/canboat [3] http://signalk.org [4] http://openskipper.org [5] http://macenc.com [6] http://www.polarnavy.com [7] https://en.wikipedia.org/wiki/NMEA_2000 [8] http://forum.openmarine.net/forumdisplay.php?fid=11


