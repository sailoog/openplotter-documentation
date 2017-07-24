# USB WiFi Stick

![](../en/wifi.png)

Je kan Openplotter of als access point instellen om apparaten connectie te laten maken of als client om zelf connectie met een Acces point te maken. Het is niet mogelijk om dit tegelijkertijd met een enkele WiFi apparaat te doen. Om dat wel te doen heb je een extra USB WiFi stick nodig voor een Raspberry 3 en twee USB WiFi devices voor een Raspberry 2.
Als Rpi verbonden is met een accesspoint als client om een internet verbinding te maken en tegelijk Openplotter zelf als access point functioneert, dan kan je de internet connectie delen met alle met openplotter verbonden apparaten. 

Een goede WiFi stick gebruikt waarschijnlijk meer stroom dan een USB poort van de Raspberry kan leveren, met name as er een grote afstand overbrugt moet worden, of wanneer er grote hoeveelheden data verstuurd worden. Om deze reden zal je waarschijnlijk de WiFi stick middels een gevoede USB hub moeten aansluiten.  

Niet alle WiFi stick kunnen als access point functioneren, alleen dongels met de juiste chipset zullen werken. Wij adviseren een  **RTL8192CU/CUS** chipset.

## Settings

Zie het [WiFi AP](/wifi-ap.md) hoofdstuk om OpenPlotter als client of access point te configureren.
