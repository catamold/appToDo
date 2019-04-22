---
title: Data Received
parent: Weather API
grand_parent: Iteration 2
has_children: false
---

## Data Received

Example of JSON data file received from [OpenWeatherMap](https://openweathermap.org/current):

	"coord":{"lon":23.59,"lat":46.77},
	"weather":[{"id":803,"main":"Rain","description":"light rain","icon":"04d"}],
	"base":"stations",
	"main":{*"temp":287.65,"pressure":1019,"humidity":47,"temp_min":287.04,"temp_max":288.15},
	"visibility":10000,
	"wind":{"speed":5.7,"deg":100},
	"clouds":{"all":75},
	"dt":1555936200,
	"sys":{"type":1,"id":6913,"message":0.0047,"country":"RO","sunrise":1555903578,"sunset":1555953707},
	"id":681290,
	"name":"Cluj-Napoca",
	"cod":200

The following field will be processed so that it will give some advice to user:
* **weather.main**: _Rain (/Snow)_
* **main.temp**: _287.65 'F
* **visibility**: _10000_ m
* **wind.speed**: _5.7_ m/s
* **clouds.all**: _75_ / 100 
* **name**: _Cluj_Napoca_

From these information we can say if it's raining or snowing or if it's a sunny day or cloudy based on percentage of cloud cover. Horizontal visibility will tell us if the weather is foggy and finally the wind speed can give us information about storms or hurricane.
