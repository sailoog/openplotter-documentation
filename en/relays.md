# Relays
---

This chapter is under construction

---

The GPIO pins can only deliver a few mA, and cannot drive directly a relay. Therefore a few electronics components are required : 

![](Relay.jpg)

* The NPN transistor BC54x acts as a valve to control the current through the relay coil (switching mode) : it is either passing when GPIO is HIGH, or blocked when GPIO is LOW. Its maximum current is 100 mA ;
* The 1 kOhm resistor limits the current drawn from the GPIO pin below 3 mA ; 
* The diode, 1N4007 prevents damaging the transistor (and/or GPIO pins !) when the relay is commuted. 
* The relay is a 5VDC relay, with an internal resistance of 60 Ohm. It requires less than 90mA compatible with the transistor. (e.g. printed circuit relay Omron G5RL-1-E-HR 5 VDC 5 V/DC 16 A ). It is available from Conrad on line shops. 

Relays used in automobile industry should be connected to + 12 VDC. They will draw a higher current (4 to 500 mA), and call for a more elaborated design (cascading two transistors). 





