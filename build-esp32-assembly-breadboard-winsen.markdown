---
layout: default
title:  Winsen MH-Z19B, MH-Z19C & MH-Z194
permalink: /make/esp32/assembly/winsen/MHZ1x
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ESP32
      url: /make/esp32
    -
      name: Assembly
      url: /make/esp32/assembly
    - 
      name: Winsen MH-Z19B, MH-Z19C & MH-Z194
---
### Bill of Materials

|Part|Voltage|Protocol|Required|
|--|--|--|--|
|2xMini Breadboard|||Yes|
|ESP32-WROOM32|5V||Yes|
|BME280|3.3V|I2C|Yes|
|SSD1306|3.3V|I2C|Yes|
|MB85RC256V|3.3V|I2C||
|MH-Z19B, MH-Z19C or MH-Z194|5V|UART|Yes|


### Diagram

<img src="https://i.ibb.co/hVVGJqX/breadboard.png" style="width:auto" height="400" alt="Diagram of AirMeter.io device built on two breadboards using a Winsen sensor"/>


### Prepare breadboards
To accommodate the dimensions of CO2 sensor and ESP32-WROOM32 the two breadboards can be clipped together. 

First remove the power rail from one side of each breadboard. Then clip the two boards together so that there are no power rails in the center. 

Finally place one of the spare power rails that were removed onto the side of the connected boards. This second power rail will be used as the I2C bus.

### Use a power rail to connect 3.3V and GND
Connect a 3.3V (+) pin and GND (-) pin of the ESP32-WROOM32 to an unused power rail +/- pair on the breadboard. 

Next connect the matching VCC (3.3V) and GND (-) pins on the components listed below to the matching rail which is connected to the ESP32-WROOM32:
- BME280
- SSD1306 display
- MB85RC256V FRAM (optional)

### Use a another power rail as an I2C bus
Nominate a second power rail pair to use as an I2C bus. 

Connect D22 (SCL) on the ESP32-WROOM32 to one rail in the pair and then connect D21 (SDA) to the other. 

Then for each of the components listed below connect the matching SCL and SDA pins to the matching rail connected the corresponding pins on the ESP32-WROOM32:
- BME280
- SSD1306 display
- MB85RC256V FRAM (optional) 

### Connect 5V power and GND to Winsen Sensor
This sensor requires a 5V as it's supply voltage. Therefore connect the VCC and GND pins directly to the 5V and GND pins on the ESP32-WROOM32.


### Connect the Winsen sensor using UART
Connect the RX and TX pins on the CO2 sensor to RX2, TX2 respectively on the ESP32-WROOM32.
