## A Heltec Wifi kit 32 (V3) and WS2812b LED Parking Assistant

![Four_Bars_ExtraSmall](https://user-images.githubusercontent.com/55962781/202794373-1cdfc5d2-508c-4eeb-9bc8-bf75e5dc39d9.jpg)

A simple to build and use garage parking assistant using an ESP8266 or ESP32 and WS2812b LEDs.  Using a low cost Wemos D1 Mini or ESP32 Mini, a short strip of around 20-40 WS2812b LED pixels and TFMini-s LIDAR distance sensor, a visual parking assistant system for putting your car in the same location in the garage each time can easily be created.

### ESP8266 Support Has Ended (v0.52+)

Due to the continued addition (and complexity) of new features, it has unfortunately become necessary to drop support for the ESP8266 beginning with release v0.52.  If you have or wish to use an ESP8266, then you must use firmware v0.51 or earlier.  I've tried to update the wiki and related pages, but if you still see references to the ESP8266 please be aware that this applies to firmware v0.51 or earlier.  Newer features shown in the wiki and discussed elsewhere also may not be available in the older ESP8266 versions.  It is highly recommended to now use an ESP32 for all new builds.

### Please see the [wiki](https://github.com/Resinchem/ESP-Parking-Assistant/wiki) for full details on installation, configuration, settings and options.
If you just want to install the firmware for the ESP8266/ESP32, **[download the appropriate .bin file from the Releases page](https://github.com/Resinchem/ESP-Parking-Assistant/releases/latest)**.  You do not need to download anything from the /src folder nor do you need to clone the repository.  Please follow the wiki instructions before asking questions about how to install the software.

Some key features of the system include:
- 4 variable distance parking zones, including a wake zone, an active zone, a parked zone and a backup zone.
- Each zone can have its own unique LED color, specified by the user
- The active zone has 5 different approach effects that can be used to visually show the car approaching the final parked position
- Automatically goes to standby or sleep mode and only awakens when a car enters the wake zone
- Supports any number of LED pixels, up to 100, and is designed so the LED strip can be mounted horizontally or vertically
- All options and settings made through a web interface
- Over-the-air firmware updates, with a manual OTA option available for uploading your own modified source code
- **Optional** MQTT integration so you can use the parking assistant in Home Assistant or other automation systems
- **Optional** Lateral guidance via a secondary sensor (v0.50+ / ESP32 versions only)


**Note**: This repo only deals with the firmware/software application. For an overview of the build details and to see some of the features in use, please see this original [YouTube video](https://youtu.be/HqqlY4_3kQ8).

**Update**: For information regarding the v0.50 update, including ESP32 support and the addition of lateral guidance via a secondary sensor, watch this [YouTube Video Update](https://youtu.be/Eps6QCgKzaM ) (the update video only covers the new features and not the full build).

Full step-by-step build instructions, including parts lists, wiring diagrams and more can be found in my blog article: [A New Parking Assistant using an ESP8266/ESP32 and WS2812b LEDs](https://resinchemtech.blogspot.com/2022/11/esp-parking-assistant.html)

It takes substantial time, effort and cost to develop and maintain this repository. If you find it helpful and would like to say 'thanks', please consider supporting this project and future development:

<a href="https://www.buymeacoffee.com/resinchemtech" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>

