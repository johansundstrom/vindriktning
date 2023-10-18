# Vindriktning till Home Assistant

## BOM

* IKEA Vindriktning
* WeMos D1 Mini eller liknande

## IKEA Vindriktning

* (fynd ~100SEK) https://www.ikea.com/se/sv/p/vindriktning-luftkvalitetsmaetare-70498242/
* Mäter PM25 (particulate matter 2.5µg/m^2^ )
* Drivs med 5VDC från USB-C, ingen spänningsregulator på kortet

## WeMos D1 Mini

* Arkitektur: ESP8266
* Spänningsregulator: inbyggd (5-3V3)
* USB-C
* CP2104 USB-UART

## Anslutning

| Vindriktning | D1 Mini |
|--|--|
| +5V | +5V |
| GND | GND |
| REST | D2 |

## Tasmota

* Kompilera egen Tasmota och inkludera ```USE_VINDRIKTNING``` i ```user_config_override.h``` 
