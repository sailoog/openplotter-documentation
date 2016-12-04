# SignalK Simulator

![](/en/SKsimulator.jpg)

Select the values you want. You can see your simulated values on SignalK **Diagnostic**.

You can use other SignalK values by editing the file _SK-simulator.conf. _It can be accessed by the setting buttom.

_\[main\]_

_item\_0 = \[0, 'navigation.courseOverGroundTrue', 0, 0, 360, 0.0174533, 0\]_

_item\_1 = \[1, 'navigation.speedOverGround', 4, 0, 10, 0.5144441, 0\]_

_item\_2 = \[2, 'navigation.headingMagnetic', 0, 0, 360, 0.0174533, 0\]_

_item\_3 = \[3, 'environment.wind.angleApparent', 0, -180, 180, 0.0174533, 0\]_

_item\_4 = \[4, 'environment.wind.speedApparent', 4, 0, 40, 0.5144441, 0\]_

_item\_5 = \[5, 'environment.wind.angleTrueWater', 0, -180, 180, 0.0174533, 0\]_

_item\_6 = \[6, 'environment.wind.speedTrue', 4, 0, 40, 0.5144441, 0\]_

_item\_7 = \[7, 'environment.depth.belowTransducer', 4, 0, 40, 1, 0\]_

The numbers behind the SignalK string copied from first line \(_0, 0, 360, 0.0174533, 0\)_

are:

* default value: 0


* minimum value: 0


* maximum value: 360


* factor: 0.0174533                \(PI/180 for converting deg to rad\)


* offset: 0                                \(interesting for Fahrenheit\)




