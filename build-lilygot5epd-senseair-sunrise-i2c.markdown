---
layout: default
title: Senseair Sunrise Sensor Assembly
permalink: /make/sensor-assemblies/sunrise
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
      name: Senseair Sunrise (I2C)
---

### Overview

This page describes how to build the Sensor Assembly for a Senseair Sunrise CO2 sensor. This board connects to a LilyGO 2.13in EPD displayboard via a right angle pin header mounted on the board.

Once completed this part will appear in as shown in the image below.
<img src="/buildimages/v1.0/sunrise-finished-top.jpg" style="width:auto" height="324" alt="Completed Sensor Assembly for a Senseair Sunrise CO2 sensor"/>



### Parts

|Part|Description|Quantity|
|--|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|1|
|006-0-0007|Senseair Sunrise CO2 sensor|1|
|BME280-5V|BME280 breakout board the 4 pin version which is usually labeled as supporting 5v due to the regulator used|1|
|2.54mm socket|4 Way 1 Row Straight PCB Socket 
Through Hole|2|
|2.54mm socket|5 Way 1 Row Straight PCB Socket 
Through Hole|1|
|2.54mm pin header|8 Way, 1 Row, Right Angle Pin Header|1|
|Wire|Six colors of wire.|

### Wire Colors

|Color|Purpose|
|--|--|
|Black|Ground|
|Red|3.3v|
|Blue|I2C SDA|
|Green|I2C CLK|
|White|Reading Ready|
|Yellow|Enable Sensor|


### Build Steps 

#### Step 1 - Attach the 8 way right angle pin header

Get the following parts ready before starting this step.

|Part|Description|Quantity|
|--|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|1|
|2.54mm pin header|8 Way, 1 Row, Right Angle Pin Header|1|

<img src="/buildimages/v1.0/sunrise-step1-parts.jpg" style="width:auto" height="400" alt="Parts required for step 1 of assembly"/>

At one thin (10 holes/3cm wide) end of the PCB attach the pin header to the PCB using solder. The pins must face inwards towards the other thin end of the PCB. 

After completing this step the PCB should appear as in the the image below.

<img src="/buildimages/v1.0/sunrise-step1-output.jpg" style="width:auto" height="400" alt="PCB after step 1 has been completed"/>


#### Step 2 - Attach 4 way PCB Socket for BME280 board

Get the following parts ready before starting this step.

|Part|Description|Quantity|
|--|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|1|
|2.54mm socket|4 Way 1 Row Straight PCB Socket 
Through Hole|1|

<img src="/buildimages/v1.0/sunrise-step2-parts.jpg" style="width:auto" height="354" alt="Parts required for step 2 of assembly"/>

Orientate the PCB so that the PIN header is underneith and on the right hand side. 

At the bottom and six holes in from the right of the PCB mount the 4 way socket using solder.

The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step2-output.jpg" style="width:auto" height="400" alt="PCB after step 2 has been completed"/>


### Diagram

<img src="https://i.ibb.co/B2pkZxP/breadboard-sunrise.png" style="width:auto" height="400" alt="Diagram of AirMeter.io device built on two breadboards using an SenseAir Sunrise"/>


### Prepare the breadboards
To accommodate the dimensions of CO2 sensor and ESP32-WROOM32 the two breadboards can be clipped together. 

First remove the power rail from one side of each breadboard. Then clip the two boards together so that there are no power rails in the center. 

Finally place one of the spare power rails that were removed onto the side of the connected boards. This second power rail will be used as the I2C bus.

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
- Senseair Sunrise




