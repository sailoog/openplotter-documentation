# Actions

Here you can activate reactions on events.

An event can be:

* SignalK data or timestamp or source
* Date

typical examples for events

If GPIO inputs are setup. They are displayed in SignalK \(Diagnostic\) when status changed.

#### An event can be:

* pushing a buttom which is connected to GPIO
* if a temperature rises over a level
* if the pressure drops under a level
* if a Signal K data wasn't updated in a time \(lost\)
* if the tank level drops under a level
* if battery voltage drops under a level
* if depth is lower then a level
* if speed is higher then a level
* ...

#### The action which is triggerd when the event occurs can be:

* play a sound \(alarm, ...\)
* Set Signal K key value \(GPIO, alarm, ...\)
* show message
* any command \(some commands can be directly taken from the list. Command line commands must be entered\)

An example with temperature. When Temperature rises over 25 °C you want to be warned by a Message and a Signal K notification key should get the value 1.

If the temperature drops under 24 °C a warning message should pop up and the notification key should get value 0.

\(don't forget that Signal K values are in SI unit in this case Kelvin\)

![](/en/Action1.jpg)

![](/en/Action_edit.jpg)

![](/en/Action2.jpg)

This example demonstrates the usage

