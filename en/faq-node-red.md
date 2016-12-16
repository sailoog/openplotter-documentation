Q: Is there also a chance to send values to the SignalK server of OpenPlotter?

A: Yes you can send values to the server when you use the minimum SignalK JSON format. For example:

```json
{
	"updates": [{
			"source": {
				"type": "ARMTEMP",
				"src": "RPIMCU"
			},
			"values": [{
					"path": "environment.inside.heating.temperature",
					"value": "323.15"
				}
			]
		}
	]
}

```
In this example we want to send the RPI cpu temperature to the SignalK Server.

![](/assets/node-red send cpu temp.jpg)

![](/assets/node-red send temp diag.jpg)

We diidn't fin