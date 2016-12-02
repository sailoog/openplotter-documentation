## Signal K

Is the base protocol of OpenPlotter.

It is optimized for Internet browser. The data stream depend on json format.

both NMEA formats are converted to SK. The format is open and the values are readable. It uses strict SI-units.

On the SignalK tab you can enter the MMSI of the boat and "apply changes".

# Diagnostic

SignalK diagnostic

![](/assets/SK-diagnostic.jpg)

Data can be sorted by source or by SignalK.

To change the units click on Unit  Setting

If private Unit is unchecked standard SI-units are shown.

# SignalK Simulate

tools-&gt;SignalK Simulator

It's a tool which streams Data to the SignalK server. You can test it with Diagnostic.

There is a ".conf" file which is opened by the setting buttom

item\_8 = \[8, 'environment.wind.speedApparent', 4, 0, 40, 0.5144441, 0\]

\[Position in the GUI,SignalK-name,default value, min value, max value, multiplier, offset\]

So it's easy to edit.

Start the GUI with the start buttom. The window is resizeable. Don't use more than 4 config lines on a small display.

!!! Never use this tool while sailing or boating !!!

