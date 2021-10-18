---
layout: default
title: Breadboard Assembly Instructions
permalink: /make/esp8266/breadboard_assembly
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ESP8266
      url: /make/esp8266
    -
      name: Breadboard Assembly Instructions
---

## Build Instructions

There are two designs described in this document which one to use depends on which CO2 sensor you are using. The designs are explained in using the steps to be followed

if building on a breadboard. Clearly as long as the same connections are maintained these can be built using a PCB or directly soldered wires.

Both designs utilise a power rail (+/-) for power distribution at 3.3V and another power rail as an I2C bus.

### Using all I2C (Senseair Sunrise)

All components in this build using 3.3V so so first connect a 3.3v (+) pin and ground (-) pin of the NodeMCU to a power rail +/- pair on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise to the matching power rail in the pair just connected to the NodeMCU.

Next nominate another different power rail pair as an I2C bus. Connect D2 (SCL) on the NodeMCU to the first rail in the pair and then connect D1 (SDA) to the second rail in the pair. Then for the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise connect the matching SCL and SDA pins to the matching rails you just connected the corresponding pins on the NodeMCU.

Do NOT connect the VV (5v from USB) pin on the NodeMCU to anything unlike the alternative build.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/B2pkZxP/breadboard-sunrise.png)

### Using UART for CO2 Sensor (Winsen and Cubic sensors)

The SSD1306 display, MB85RC256V FRAM (optional) and the BME280 sensor both use I2C and operate at 3.3v. So first connect a 3.3v (+) pin and a ground (-) pin of the NodeMCU to a power rail (+/- pair) on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280 and SSD1306 display to the matching power rail in the pair just connected to the NodeMCU.

Use another different power rail pair as an I2C bus. Connect D2 (SCL) on the NodeMCU to the first rail in the pair and then connect D1 (SDA) to the second rail in the pair. Then for both the BME280, MB85RC256V FRAM (optional) and the SSD1306 connect the match SCL and SDA pins to the matching rail you just connected the NodeMCU.

Connect the VV (5v from USB) pin on the NodeMCU to the VCC (5v) pin on the CO2 sensor and connect the GND pin on the sensor to a GND pin on the NodeMCU.

Finally connect the RX pin on the CO2 sensor to D8 on the NodeMCU and the TX pin on the CO2 sensor to D7 on the NodeMCU.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/hVVGJqX/breadboard.png)


