---
layout: default
title: Portable CO2 monitor with an ePaper display
permalink: /make/epd213
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ePaper
---

<img src="/buildimages/v1.0/finished-device.jpg" style="width:auto" alt="Complete ePaper CO2 monitor"/>

This section describes how to build a portable battery operated device with an electronic paper display. 

See the following subsections for a brief outline of each part of the build process and links to further detail.

### [Sensor Assembly](/make/sensor-assemblies/sunrise)
This is a 7cm x 3cm PCB on which the sensors are mounted. On the underside which is exposed when it is screwed in place is a 8 way right angle male PCB connector to connect to the LILYGO® TTGO T5 V2.3.1_2.13 board.

### [Prepare LILYGO® TTGO T5 board](/make/epd213/prepare)
The LILYGO® TTGO T5 V2.3.1_2.13 board provides the following in one package:
- An ESP32, antenta and flash.
- A 2.13in ePaper SPI display.
- Battery control circuitry.

This board must have an 8 way connector andwires soldered to it to acts as a cable to connect to the sensor assembly.

### [3D print case & assemble](/make/epd213/assemble)
The case must be printed using a suitable 3D printer. The LilyGO board and sensor assembly must be assembled in a specific order.

