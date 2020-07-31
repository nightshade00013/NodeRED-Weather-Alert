# NodeRED-Weather-Alert
A NodeRED flow that will alert you when bad weather is coming through your area.


If you found this project helpful and want to throw a few bones my way I would greatly appreciate it. You have a couple options to do so. One is to make a purchase on Amazon using my affiliate link, donate through buy me a coffee, or toss a couple Satoshi to me using Bitcoin.

https://amzn.to/2v74aiY Amazon affiliate link, any purchases made after clicking this will help support the author. https://www.buymeacoffee.com/Slw0NRx donation link through Buy Me a Coffee. 17pEPchqZrjVHv8oN3jKMDZp23A24j4Jj Bitcoin address for direct anonymous gifts.

This works with NodeRed and Home Assistant to control RGBW Tuya based bulbs that have been flashed to ESPHome. It may also work with other bulbs and other firmware but I can not guarantee or assist with that.  I am also using Sonoff based switches that are flashed to ESPHome.  Remember you must setup your Home Assistant in Node-Red and your API key in OpenWeatherMap.

Outside of the inbuilt nodes I used the used nodes node-red-contrib-home-assistant-websocket, node-red-node-openweathermap .

This is placed for use by others who may be interested and want to try it. It comes with no support or guarantee.

https://esphome.io/cookbook/teckin_sb50.html information for the Tuya based Bulbs and the basic YAML used for compiling.

https://www.home-assistant.io/ Home Assistant.

https://nodered.org/ NodeRed.

https://github.com/ct-Open-Source/tuya-convert Software to flash bulbs to ESPHome.

https://esphome.io/ ESPHome main page.

When you configure for your particular weather condition you will want to go to https://openweathermap.org/weather-conditions and then pull the weather ID's you are worried about.  Depending on your location that could be just about anything but for instance my area has Tornadic activity so the code 781 is used for Tornado.  If you are worried about sandstorms 751 would be the correct code or if you have a volcano nearby you would use 762.  For major thunderstorms you might use both 212 and 221 which could be put as two outputs or a single "between" range since no other codes fall between them.  You could even expand to using only RGB bulbs and have a particular weather condition be displayed at the end of the flashing by a particular color or have the bulb flash with a particular color.  The possibilities are truly endless but this should get you on the way.

