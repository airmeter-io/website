---
layout: default
title: Senseair Sunrise (UART)
permalink: /make/esp8266/assembly/senseair/sunrise-uart
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ESP8266
      url: /make/esp32
    -
      name: Assembly
      url: /make/esp8266/assembly
    - 
      name: Senseair Sunrise (UART)
---
### Parts

|Part|Voltage|Protocol|Required|
|--|--|--|--|
|2xMini Breadboard|||Yes|
|NodeMCU|5V||Yes|
|BME280|3.3V|I2C|Yes|
|SSD1306|3.3V|I2C|Yes|
|MB85RC256V|3.3V|I2C||
|Senseair Sunrise|3.3V|UART|Yes|


### Diagram

<img src="https://i.ibb.co/B2pkZxP/breadboard-sunrise.png" style="width:auto" height="400" alt="Diagram of AirMeter.io device built on two breadboards using an SenseAir Sunrise"/>


### Prepare the breadboards
To accommodate the dimensions of CO2 sensor and NodeMCU the two breadboards can be clipped together. 

First remove the power rail from one side of each breadboard. Then clip the two boards together so that there are no power rails in the center. 

Finally place one of the spare power rails that were removed onto the side of the connected boards. This second power rail will be used as the I2C bus.

### Use a power rail to connect 3.3V and GND
Connect a 3.3V (+) pin and GND (-) pin of the NodeMCU to an unused power rail +/- pair on the breadboard. 

Next connect the matching VCC (3.3V) and GND (-) pins on the components listed below to the matching rail which is connected to the NodeMCU:
- BME280
- SSD1306 display
- MB85RC256V FRAM (optional)
- Senseair Sunrise

### Use a another power rail as an I2C bus
Nominate a second power rail pair to use as an I2C bus. 

Connect D2 (SCL) on the NodeMCU to one rail in the pair and then connect D1 (SDA) to the other. 

Then for each of the components listed below connect the matching SCL and SDA pins to the matching rail connected the corresponding pins on the NodeMCU:
- BME280
- SSD1306 display
- MB85RC256V FRAM (optional) 

### Connect the Sunrise sensor using UART
Connect the RX and TX pins on the CO2 sensor to D8, D7 respectively on the NodeMCU.



