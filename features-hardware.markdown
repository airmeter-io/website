---
layout: default
sortOrder: 3
permalink: /features/hardware
title: Hardware
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Hardware  
---

### Microcontrollers
*ESP32* & *ESP8266* families of MCUs made by *Espressif* are the supported platforms presently. Both chip families have a wide range of boards available in different form factors and bundled peripheral components.

The supported microcontrollers are:
- ESP32
- ESP32-S2
- ESP32-C3 
- ESP32-S3 
- ESP32-C6
- ESP8266. 

These were chosen due the popularity of these MCUs with makers and existing CO2 monitoring projects. 

### Pressure, temperature and humidity sensor

The supported sensors at this time are:
- Bosch BME280
- Bosch BMP280

These sensors provides temperature, pressure and humidity readings. It can be substituted with a *GY-BMP280* if required. The *BME280* is presently in short supply.

### Display
The display is used to enable secure WiFi provisioning, display live readings and provide on-device menus.

#### SSD1680 driven ePaper 
ePaper is an excellent choice for battery operated devices that are used in varied light conditions as it is low power and a reflective display technology.

At present *AirMeter.io* supports the following SSD1680 driven ePaper displays, others will be added in time:
- DEPG0213BN

The LilyGo 2.13 ESP32 ePaper Display board can be used an excellent based for an *AirMeter.io* device and includes a supported display, battery charging hardware and an mini SD card reader.


#### SSD1306 128x64 OLED/LCD
This is a cheap and easily sourced display that can be connected via I2C. Whilst limited in size it is sufficient to display readings.

### CO2 Sensor

#### Senseair Sunrise

The *Senseair Sunrise* is an excellent sensor and has been a primary focus of testing and development due to its recognised use is premium commercial devices.

This sensor can be connected either via I2C or UART. At present the UART implementation is considered most stable and should be preferred. 

It is Grade A 3.3v sensor suitable for battery operated devices.

#### Sensirion SCD30
The *SCD30* has been popular in many existing DIY CO2 sensor projects. Therefore *AirMeter.IO* provides full support for this sensor operating over I2C.

It is a 3.3v sensor suitable for battery operated devices.

#### Cubic CM1107/CM1106
Cubic are reported to produce high quality sensors and *AirNeter.io* has full support for these sensors. However as all testing has been performed on second hand units AirMeter.io, it is impossible to comment further.


#### Winsen MH-Z19B/C & MH-Z14
The *Winsen MH-Z19B/C* sensors are fully supported and tested "functionally". Results may vary but it is worth noting that:
- These sensors generally require forced background calibration.
- Voltage and quality of power supply maybe important.

The MH-Z14 sensor has been lightly tested but has not been deeply investigated and tested.

### Battery (Strongly Recommended)
Using an ESP32 or ESP8266 board with battery/power management support is preferable as then it allows the inclusion of a lithium ion battery which achieves two important things:
- Device portability as it does not need to be tethered to a power source.
- Reliable power ensuring readings are not missed which adds utility even where portability is not required.

It is possible to build your owner battery/power management circuitry if you have the appropriate skills/knowhow but the easiest method is to purchase a board with this built in.


### Enclosure and Electrical Connections
Within the build section examples are given with 3D printable parts showing how to soldier and assemble fully functional battery operated portable devices. 

If you are designing your own device then generally speaking one must ensure that:
- Electrical connections are competently soldiered.
- Sensor manufacturer guidelines relating to clearances and mounting are followed.
- Power is suitably managed either by an off the shelf board or otherwise. This may be a particular challenge if using 5V sensors.

