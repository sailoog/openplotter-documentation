# Sending data to the autopilot

The autopilot has to be setup

![](/en/setup-autopilot-window.jpg)

Click on add \(or double click on auto\_ap\).

![](/en/setup-autopilot-window1.jpg)

Click on AP examp to load default settings for autopilot.

![](/en/setup-autopilot-window2.jpg)       ![](/en/setup-autopilot-window3.jpg)  
                                                                                                                                                         Select port ttyOP\_AP

in Filter: What sentences are allowed to be received from the autopilot to OpenPlotter/kplex.

Most autopilots have there own fluxgate compass and rudder angle sensor. These data can be used from openplotter.

More important is the

out Filter: What sentences are allowed to be send from OpenPlotter/kplex to the autopilot.

It is important to filter the sentences to reduce the transfer volume. NMEA0183 autopilots work normally with 4800 bauds. There's only space for a few sentences.

Which sentences are important?

* RMB \(way to selected waypoint send from a chartplotter\)

* RMC \(minimum GPS data\)

* VHW \(waterspeed and heading\)

* VWR \(wind\)

* sometimes APA and APB




