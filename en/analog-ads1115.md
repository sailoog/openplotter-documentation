# Analog ads1115

Is an adc with:

* 4 inputs

* 16 bit

* selctable gain

* selectable sample rate


When selected settings the configuration file will be opened.

_\[ADS1115\_0\] active = 1  
gain = 0   
samples = 6   
ohmmeter = 0   
fixed\_resistor = 0   
high\_voltage = 3000   
voltage\_divider = 0   
upper\_resistance = 1000   
lower\_resistance = 1000   
adjust = 0   
sk\_name = tanks.fuel.left.currentLevel   
adjust\_points = \[\[100.0,0.0\],\[5000.0,90.0\],\[9000.0,100.0\]\]  
_

If a channel is used active must be set to 1

The gain setting can be changed with gain.

gain = 0 +/- 6.144V

gain = 1 +/- 4.096V

gain = 2 +/- 2.048V

gain = 3 +/- 1.024V

gain = 4 +/- 0.512V

gain = 5 +/- 0.256V

samples setting can be changed with samples \(see table\).

samples 0 8  samples per second

samples 1 16 samples per second

samples 2 32 samples per second

samples 3 64 samples per second

samples 4 128 samples per second

samples 5 250 samples per second

samples 6 475 samples per second

samples 7 860 samples per second

ohmmeter can be set to 1 to measure the resistance of a sensor.

fixed\_resistor must be set to the resistance of the fixed resistor and

high\_voltage is the voltage you put on the two resistors in serial.

The resistance you want to measure is connected on one side to ground and

on the other side to the fixed resistor and analog input of the adc.

The other side of the fixed resistor is connected to + pol \(for example 3.3V \(high\_voltage\)\)

voltage\_divider can be set to 1 if you want to have Volt values.

If you want to measure 12 V with a adc witch is only capable of max 3.3V,

you need a voltage divider in form of two resistors. \(50k+10k would put the voltage from 12V to 2V\)

upper\_resistance has to be set to 50000 and lower resistance to 10000 for this example.

Look at the picture on [http://forum.arduino.cc/index.php?topic=214930.0](http://forum.arduino.cc/index.php?topic=214930.0)

adjust is only for adjusting the offset

The value is send to SignalK on the name you set in sk\_name.

adjust\_points

You can put in some points of a curve.

Between this point the value is calculated linear.

This is the easiest way to get good results.

It can be used in combination with voltage\_devider or ohmmeter.

