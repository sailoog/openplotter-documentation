# Switches

---

This chapter is under construction

---
Switches are driven through the GPIO (General Purpose Input/Output) pins. These pins are copper connected to the CPU chip. A short circuit with 0V or +3.3V is not final, but any direct contact with the + 5v (or higher) can KILL the Raspberry Pi... Switches have to be activated in OpenPlotter related tab. 

For normal switches (opened by default), you have to select "Pull down" in "Switches" tab an connect switch between selected GPIO pin and +3.3v pin (DANGER, NEVER TO +5v). 

For special switches (closed by default), you have to select "Pull up" in "Switches" tab an connect switch between selected GPIO pin and GND pin.

It is not a problem if you make a mistake connecting to GND or +3.3v but be careful and avoid +5v pin. 

Pins numbers are according to the diagram below where, for example, pin GPIO22 is pin position number 15.

![](RP2_Pinout.png)