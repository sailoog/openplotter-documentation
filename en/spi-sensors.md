## SPI

The adc \(analog digital converter\) MCP3008 is implemented in openplotter.

![](/en/mcp3008.jpg)

It does read voltage between 0 - 3.3V. It is has a 10bit resolution \(0-1023\).

Many signals aren't linear. To get a nearly linear result you can use the value setting.

![](/en/mcp3008form1.jpg)

The medium level in a tank on boats isn't linear to the hight the sensor measures. To calibrate it emty it and insert the adc value for 0%. fill in 10% of max volume and insert adc value and 10.0. Go on untill the tank is full.

Look at the graph you created by clicking on graph

![](/en/mcp3008graph1.jpg)