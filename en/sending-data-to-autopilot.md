# Sending data to the autopilot

The autopilot has to be setup ![](/assets/screenshot.98.jpg)

Click on add \(or double click on auto\_ap\).

![](/assets/screenshot.100.jpg)

Click on AP examp to load default settings for autopilot.

![](/assets/screenshot.101.jpg)       ![](/assets/screenshot.102.jpg)

                                                                                                                                                           Select port ttyOP\_AP

in Filter: What sentences are allowed to be transfered from the autopilot to openplotter/kplex.

Most autopilots have there own fluxgate compass and rudder angle sensor. These data can be used from openplotter.

More important is the 

out Filter: What sentences are allowed to be transfered from openplotter/kplex to the autopilot. 

It is important to filter the sentences to reduce the transfer volume. NMEA 0183 autopilots work normally with 4800 bauds. So there's only space for a few sentences. 

Which sentences are important?

* RMB \(way to selected waypoint send from a chartplotter\)

* RMC \(minimum GPS data\)

* VHW \(waterspeed and heading\)

* VWR \(wind\)

* sometimes APA and APB




