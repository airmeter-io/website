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

There are three designs described here, use the one for the CO2 sensor being used. One important difference between sensors is 3.3V and 5V it is essential that the right design is chosen.

For ease of understanding the builds are explained as if they are built on a breadboard. As long as the components are connected in same manner a PCB, directly soldered wires or any other reliable electric connection can be used. Breadboards ARE NOT recommended for devices which see active use.

All three designs utilise a power rail (+/-) for 3.3V power distribution and another power rail (if using a breadboard) as an I2C bus.

### UART with the 3.3v Senseair Sunrise sensor

All components in this build using 3.3V so so first connect a 3.3V (+) pin and ground (-) pin of the NodeMCU to a power rail +/- pair on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise to the matching power rail in the pair just connected to the NodeMCU.

Next nominate another different power rail pair as an I2C bus. Connect D2 (SCL) on the NodeMCU to the first rail in the pair and then connect D1 (SDA) to the second rail in the pair. Then for the BME280, SSD1306 display and MB85RC256V FRAM (optional) connect the matching SCL and SDA pins to the matching rails you just connected the corresponding pins on the NodeMCU.

Finally connect the RX pin on the CO2 sensor to D8 on the NodeMCU and the TX pin on the CO2 sensor to D7 on the NodeMCU.

Do NOT connect the VV (5V from USB) pin on the NodeMCU to anything.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/B2pkZxP/breadboard-sunrise.png)

### I2C with the 3.3V Senseair Sunrise sensor

All components in this build using 3.3V so so first connect a 3.3V (+) pin and ground (-) pin of the NodeMCU to a power rail +/- pair on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise to the matching power rail in the pair just connected to the NodeMCU.

Next nominate another different power rail pair as an I2C bus. Connect D2 (SCL) on the NodeMCU to the first rail in the pair and then connect D1 (SDA) to the second rail in the pair. Then for the BME280, SSD1306 display, MB85RC256V FRAM (optional) and Senseair Sunrise connect the matching SCL and SDA pins to the matching rails you just connected the corresponding pins on the NodeMCU.

Do NOT connect the VV (5V from USB) pin on the NodeMCU to anything.

![Schematic of a this built using two mini breadboards](https://i.ibb.co/B2pkZxP/breadboard-sunrise.png)


### Using UART on 5v Winsen (MH-Z19B/C, MH-Z14) and Cubic (CM1107/CM1106) sensors

The SSD1306 display, MB85RC256V FRAM (optional) and the BME280 sensor both use I2C and operate at 3.3V. So first connect a 3.3V (+) pin and a ground (-) pin of the NodeMCU to a power rail (+/- pair) on the breadboard. Then proceed to connect the matching VCC (+) and ground (-) pins on both the BME280 and SSD1306 display to the matching power rail in the pair just connected to the NodeMCU.

Use another different power rail pair as an I2C bus. Connect D2 (SCL) on the NodeMCU to the first rail in the pair and then connect D1 (SDA) to the second rail in the pair. Then for both the BME280, MB85RC256V FRAM (optional) and the SSD1306 connect the match SCL and SDA pins to the matching rail you just connected the NodeMCU.

Connect the VV (5V from USB) pin on the NodeMCU to the VCC (5V) pin on the CO2 sensor and connect the GND pin on the sensor to a GND pin on the NodeMCU.

Finally connect the RX pin on the CO2 sensor to D8 on the NodeMCU and the TX pin on the CO2 sensor to D7 on the NodeMCU.


![Schematic of a this built using two mini breadboards](https://i.ibb.co/hVVGJqX/breadboard.png)


