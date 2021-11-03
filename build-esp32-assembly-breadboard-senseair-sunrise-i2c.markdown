---
layout: default
title: Senseair Sunrise (I2C)
permalink: /make/esp32/breadboard_assembly/senseair/sunrise-i2c
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ESP32
      url: /make/esp32
    -
      name: Breadboard Assembly
      url: /make/esp32/breadboard_assembly
    - 
      name: Senseair Sunrise (I2C)
---

### I2C with the 3.3V Senseair Sunrise sensor

All components in this build using 3.3V so so first connect a 3.3V (+) pin and ground (-) pin of the ESP32-WROOM32 to a power rail +/- pair on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise to the matching power rail in the pair just connected to the ESP32-WROOM32.

Next nominate another different power rail pair as an I2C bus. Connect D22 (SCL) on the ESP32-WROOM32 to the first rail in the pair and then connect D21 (SDA) to the second rail in the pair. Then for the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise connect the matching SCL and SDA pins to the matching rails you just connected the corresponding pins on the ESP32-WROOM32.

Do NOT connect the VV (5V from USB) pin on the ESP32-WROOM32 to anything.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/B2pkZxP/breadboard-sunrise.png)
