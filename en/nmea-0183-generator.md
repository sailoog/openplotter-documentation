## NMEA 0183 generator

The generator is able to generate nmea sentences from SignalK values.

For example you have the value of the water temperature "environment.water.temperature" and you want to generate a NMEA 0183 sentences.

Open the window "NMEA 0183 generator" by selecting Tools-&gt;NMEA 0183 generator

![](NMEA0183gen_1.jpg)

Press "add"

![](NMEA0183gen_2.jpg)

Select the type of NMEA "Sentence" you want to generate. For the example it is MTW. It should look like this:

![](NMEA0183gen_3.jpg)

Important: the SignalK value will be converted from Kelvin to Celsius.

![](NMEA0183gen_4.jpg)

Other values can also be converted from SignalK to NMEA 0183.

When you press OK, you get back to this window.

![](NMEA0183gen_5.jpg)

Finished.

To activate the new settings SignalK tab -&gt;Restart.

## Opencpn sentences

To create the standard sentence for opencpn press "opencpn default" \(it does only work if there is no sentence\)

These SignalK values will be used:

"navigation.headingMagnetic"

"navigation.attitude.roll"

"navigation.attitude.pitch"

"environment.outside.pressure"

"environment.outside.temperature"

"environment.water.temperature"

## Use Diagnostic

To debug the result of your generated sentence go to NMEA0183 tab.

Select the line system or opencpn then click the diagnostic button. 

## Generate NMEA0183 sentences from SignalK-server

Enter the SignalK Plugins from a browser by:

openplotter.local:3000

localhost:3000

10.10.10.1:3000

![](NMEA0183SignalKgen_1.jpg)

![](NMEA0183SignalKgen_2.jpg)

![](NMEA0183SignalKgen_3.jpg)

Here you activate and select some NMEA0183 sentences. The performace is better than the NMEA 0183 generator from OpenPlotter but you have no chance to use other values, corrections or calculations.

