# Primeros pasos

Antes de nada debes reunir y conectar todas las [partes básicas](required.md). Si tienes problemas con alguna parte, intenta buscar ayuda en la [página oficial de Raspberry Pi](https://www.raspberrypi.org/help/).


A continuación, tienes que ejecutar el software en tu nuevo ordenador ARM. Usaremos **OpenPlotter RPI** que es una versión modificada de [Raspbian](https://www.raspbian.org/), el sistema operativo oficial para la Raspberry Pi.

Sigue esta guía detallada para descargar e instalar OpenPlotter RPI:

http://sailoog.dozuki.com/Guide/Descargando+e+instalando+OpenPlotter+RPI/2

O compra nuestra tarjeta SD con OpenPlotter RPI pre-instalado y listo para conectar y usar:

http://www.sailoog.com/shop-category/openplotter

## Parlez-vous français?
http://www.edelvoilier.org/themes/navigation-electronique/1408-la-rasperry-pi-comme-station-de-nav


## Ok, ¿y ahora qué?

¡Enhorabuena! Ya tiene tu sistema en funcionamiento por lo que es hora de empezar a obtener algunos datos del mundo. El paso más común y lógico sería conectar un GPS.

Es importante que entiendas que OpenPlotter debe gestionar todo el tráfico de datos para que funcione correctamente, por lo que no necesitas configurar OpenCPN para obtener señal GPS, vamos a configurarla en OpenPlotter.

Si deseas conectar un dispositivo GPS USB o un NMEA 0183 al conversor de USB, tendrás que crear una entrada en serie en el [NMEA 0183 multiplexor] (nmea_multiplexer..md).

Puedes crear entradas de red también.

Todos los datos generados por OpenPlotter ([Sensores] (sensors.md), [SDR AIS] (sdr_ais.md), [] Cálculos (calculate.md) ...) serán enviados automáticamente a * system output * (UDP localhost 10110) en el NMEA 0183 multiplexor.

Todas las entradas serán automáticamente multiplexadas y estaran disponibles en system output * * (localhost TCP 10110). Sólo tienes que configurar OpenCPN para buscar en * system output * (localhost TCP 10110) y asi obtener todos los datos.