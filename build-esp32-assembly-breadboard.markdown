---
layout: default
title: Breadboard Assembly Instructions
permalink: /make/esp32/breadboard_assembly
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ESP32
      url: /make/esp32
    -
      name: Breadboard Assembly Instructions
---

There are three designs described in this document depending on which CO2 sensor you are using. As one important difference is 3.3V and 5V it is essential that the right design is chosen.

For ease of understanding the builds are explained as if they are built on a breadboard. As long as the components are connected in same manner a PCB, directly soldered wires or any other reliable electric connection can be used. Breadboards ARE NOT recommended for devices which see active use.

All three designs utilise a power rail (+/-) for 3.3V power distribution and another power rail (if using a breadboard) as an I2C bus.

### Using all UART on 3.3v Senseair Sunrise

All components in this build using 3.3V so so first connect a 3.3V (+) pin and ground (-) pin of the ESP32-WROOM32 to a power rail +/- pair on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise to the matching power rail in the pair just connected to the ESP32-WROOM32.



Next nominate another different power rail pair as an I2C bus. Connect D22 (SCL) on the ESP32-WROOM32 to the first rail in the pair and then connect D21 (SDA) to the second rail in the pair. Then for the BME280, SSD1306 display and MB85RC256V FRAM (optional) connect the matching SCL and SDA pins to the matching rails you just connected the corresponding pins on the ESP32-WROOM32.

Finally connect the RX pin on the CO2 sensor to RX2 on the ESP32-WROOM32 and the TX pin on the CO2 sensor to TX2 on the ESP32-WROOM32.

Do NOT connect the VV (5v from USB) pin on the ESP32-WROOM32 to anything.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/B2pkZxP/breadboard-sunrise.png)

### Using all I2C on 3.3v Senseair Sunrise

All components in this build using 3.3V so so first connect a 3.3v (+) pin and ground (-) pin of the ESP32-WROOM32 to a power rail +/- pair on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise to the matching power rail in the pair just connected to the ESP32-WROOM32.

Next nominate another different power rail pair as an I2C bus. Connect D22 (SCL) on the ESP32-WROOM32 to the first rail in the pair and then connect D21 (SDA) to the second rail in the pair. Then for the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise connect the matching SCL and SDA pins to the matching rails you just connected the corresponding pins on the ESP32-WROOM32.

Do NOT connect the VV (5v from USB) pin on the ESP32-WROOM32 to anything.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/B2pkZxP/breadboard-sunrise.png)

### Using UART on 5v Winsen and Cubic sensors

The SSD1306 display, MB85RC256V FRAM (optional) and the BME280 sensor both use I2C and operate at 3.3v. So first connect a 3.3v (+) pin and a ground (-) pin of the ESP32-WROOM32 to a power rail (+/- pair) on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280 and SSD1306 display to the matching power rail in the pair just connected to the ESP32-WROOM32.

Use another different power rail pair as an I2C bus. Connect D22 (SCL) on the ESP32-WROOM32 to the first rail in the pair and then connect D21 (SDA) to the second rail in the pair. Then for both the BME280, MB85RC256V FRAM (optional) and the SSD1306 connect the match SCL and SDA pins to the matching rail you just connected the ESP32-WROOM32.

Connect the VV (5v from USB) pin on the ESP32-WROOM32 to the VCC (5v) pin on the CO2 sensor and connect the GND pin on the sensor to a GND pin on the ESP32-WROOM32.

Finally connect the RX pin on the CO2 sensor to RX2 on the ESP32-WROOM32 and the TX pin on the CO2 sensor to TX2 on the ESP32-WROOM32.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/hVVGJqX/breadboard.png)