---
layout: default
title: Senseair Sunrise (UART)
permalink: /make/esp32/breadboard_assembly/senseair/sunrise-uart
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
      name: Senseair Sunrise (UART)
---
### Bill of Materials (BOM)

|Part|Voltage|Protocol|
|--|--|--|
|ESP32-WROOM32|-|-|
|BME280|3.3V|I2C|
|SSD1306|3.3V|I2C|
|MB85RC256V|3.3V|I2C|
|Senseair Sunrise|3.3V|UART|

### Use a power rail to connect 3.3V and GND
Connect a 3.3V (+) pin and GND (-) pin of the ESP32-WROOM32 to an unused power rail +/- pair on the breadboard. 

Next connect the matching VCC (3.3V) and GND (-) pins on the components listed below to the matching rail which is connected to the ESP32-WROOM32:
- BME280
- SSD1306 display
- MB85RC256V FRAM (optional)
- Senseair Sunrise

### Use a another power rail as an I2C bus
Nominate a second power rail pair to use as an I2C bus. 

Connect D22 (SCL) on the ESP32-WROOM32 to one rail in the pair and then connect D21 (SDA) to the other. 

Then for each of the components listed below connect the matching SCL and SDA pins to the matching rail connected the corresponding pins on the ESP32-WROOM32:
- BME280
- SSD1306 display
- MB85RC256V FRAM (optional) 

### Connect the Sunrise sensor using UART
Connect the RX and TX pins on the CO2 sensor to RX2, TX2 respectively on the ESP32-WROOM32.


### Illustration of Breadboard Layout
![Schematic of a this built using two mini breadboards](https://i.ibb.co/B2pkZxP/breadboard-sunrise.png)
