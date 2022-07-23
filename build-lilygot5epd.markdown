---
layout: default
title: Battery Operated ePaper CO2 monitor
permalink: /make/epd213
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ePaper
---

<img src="/buildimages/v1.0/finished-device.jpg" style="width:auto" alt="Complete ePaper CO2 monitor"/>

This is an extremely portable CO2 monitor with great battery life even when connected to WIFI.

The design has been optimised to take advantage of the ePaper display giving live readings, graphing and the ability to calibrate just using the device itself.

As this is an *AirMeter.io* device it has the full set of web and management features that the firmware provides.

The device is made in several stages/parts which are described below.

### [Sensor Assembly](/make/sensor-assemblies/sunrise)
This is a 7cm x 3cm PCB on which the sensors are mounted. On the underside which is exposed when it is screwed in place is a 8 way right angle male PCB connector to connect to the LILYGO® TTGO T5 V2.3.1_2.13 board.

### [Prepare LILYGO® TTGO T5 board](/make/epd213/prepare)
The LILYGO® TTGO T5 V2.3.1_2.13 board provides the following in one package:
- An ESP32, antenta and flash.
- A 2.13in ePaper SPI display.
- Battery control circuitry.

This board must have an 8 way connector andwires soldered to it to acts as a cable to connect to the sensor assembly.

### [Attach 1.25mm JST connector to battery](/make/epd213/battery)
The LILYGO® TTGO T5 V2.3.1_2.13 board uses a 1.25mm pitch JST connector for the battery. The FT103450P battery must have such a connector attached.

### [3D print case & assemble](/make/epd213/assemble)
The case must be printed using a suitable 3D printer. The LilyGO board and sensor assembly must be assembled in a specific order.

