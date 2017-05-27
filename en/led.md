# LED

---

This chapter is under construction

---

## Wiring

Pins names are according to the diagram below.

![](RP2_Pinout.png)

Ignoring the Pi for a moment, one of the simplest electrical circuits that you can build is a battery connected to a light source and a switch (the resistor is there to (limit the current flow) and protect the LED):

![](simple-circuit.png)

When we use a GPIO pin as an output, the Raspberry Pi replaces both the switch and the battery in the above diagram. Each pin can turn on or off,or go **HIGH** or **LOW** in computing terms. When the pin is **HIGH** it outputs** 3.3 volts** (3v3); when the pin is LOW it is off.

Here's the same circuit using the Raspberry Pi. The LED is connected to a GPIO pin (which can output +3v3) and a ground pin which is 0v and acts like the negative terminal of the battery :
 (the resistor is there to limit the current flow and protect both the LED and the Raspberry CPU). A value of 1 kOhm will retrain the current around 1.5 mA

![](gpio-led-pi2.png)
