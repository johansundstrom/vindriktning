# Vindriktning till Home Assistant

* IKEA Vindriktning (~100SEK) https://www.ikea.com/se/sv/p/vindriktning-luftkvalitetsmaetare-70498242/
* Mäter PM25 (particulate matter 2.5µg/m2)
* Drivs med 5VDC från USB, ingen spänningsregulator på kortet

## WeMos D1 Mini

* Spänningsregulator: inbyggd
* Arkitektur: ESP8266 

## BOM

* IKEA Vindriktning
* WeMos D1 Mini eller liknande

## Anslutning

| Vindriktning | D1 Mini |
|--|--|
| +5V | +5V |
| GND | GND |
| REST | D2 |

## Tasmota

* Kompilera egen Tasmota och inkludera ```USE_VINDRIKTNING``` i ```user_config_override.h``` 
