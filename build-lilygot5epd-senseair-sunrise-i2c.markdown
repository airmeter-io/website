---
layout: default
title: Senseair Sunrise Sensor Assembly
permalink: /make/sensor-assemblies/sunrise
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ePaper
      url: /make/epd213    
    - 
      name: Senseair Sunrise (I2C)
---

## Overview

This page describes how to build the Sensor Assembly for a Senseair Sunrise CO2 sensor. This board connects to a LilyGO 2.13in EPD displayboard via a right angle pin header mounted on the board.

Once completed this part will appear in as shown in the image below.
<img src="/buildimages/v1.0/sunrise-finished-top.jpg" style="width:auto" height="170" alt="Completed Sensor Assembly for a Senseair Sunrise CO2 sensor"/>



### Parts

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|006-0-0007|Senseair Sunrise CO2 sensor|
|BME280-5V|BME280 breakout board the 4 pin version which is usually labeled as supporting 5v due to the regulator used|
|2.54mm socket|4 Way 1 Row Straight PCB Socket 
Through Hole|
|2.54mm pin header|4 Way, 1 row, straight pin header 
|2.54mm pin header|5 Way, 1 row, straight pin header 
|2.54mm pin header|8 Way, 1 row, right angle pin header|
|Wire|Six colors of wire.|

### Wire Colors

|Color|Purpose|
|--|--|
|Black|Ground|
|Red|3.3v|
|Blue|I2C SDA|
|Green|I2C SCL|
|White|Enable Sensor|
|Yellow|Reading Ready|



## Build Steps 

  - [Step 1 - Attach the 8 way right angle pin header](#step-1---attach-the-8-way-right-angle-pin-header)
  - [Step 2 - Attach 4 way PCB Socket for BME280 board](#step-2---attach-4-way-pcb-socket-for-bme280-board)
  - [Step 3 - Mounting CO2 Sensor pin headers](#step-3---mounting-co2-sensor-pin-headers)
  - [Step 4 - Attach Sunrise CO2 Sensor](#step-4---attach-sunrise-co2-sensor)
  - [Step 4 - Attach Sunrise CO2 Sensor](#step-4---attach-sunrise-co2-sensor)
  - [Step 5 - Wire 3.3V VIN (Red wire)](#step-5---wire-33v-vin-red-wire)
  - [Step 6 - Wire GND (Black wire)](#step-6---wire-gnd-black-wire)
  - [Step 7 - Wire I2C (Green and Blue wire)](#step-7---wire-i2c-green-and-blue-wire)
  - [Step 8 - Wire CO2 sensor control (White and yellow wire)](#step-8---wire-co2-sensor-control-white-and-yellow-wire)

### Step 1 - Attach the 8 way right angle pin header

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|2.54mm pin header|8 Way, 1 row, right angle pin header|

<img src="/buildimages/v1.0/sunrise-step1-parts.jpg" style="width:auto" height="200" alt="Parts required for step 1 of assembly"/>

At one thin (10 holes/3cm wide) end of the PCB attach the pin header to the PCB using solder. The pins must face inwards towards the other thin end of the PCB. 

After completing this step the PCB should appear as in the the image below.

<img src="/buildimages/v1.0/sunrise-step1-output.jpg" style="width:auto" height="154" alt="PCB after step 1 has been completed"/>


### Step 2 - Attach 4 way PCB Socket for BME280 board

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|2.54mm socket|4 Way 1 Row Straight PCB Socket Through Hole|


<img src="/buildimages/v1.0/sunrise-step2-parts.jpg" style="width:auto" height="154" alt="Parts required for step 2 of assembly"/>

<ol>
<li>Orientate the PCB so that the PIN header is underneith and on the right hand side. </li>

<li>At the bottom and six holes in from the right of the PCB mount the 4 way socket using solder.</li>
</ol>

The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step2-output.jpg" style="width:auto" height="150" alt="PCB after step 2 has been completed"/>

### Step 3 - Mounting CO2 Sensor pin headers

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|2.54mm pin header|4 Way, 1 row, straight pin header 
|2.54mm pin header|5 Way, 1 row, straight pin header 

The pin headers need to be adjusted so that the minimum length extrudes from the rear of the PCB. The pins will stick out on the PCB side to which the sensor is attached.

This is important to allow the PCB to fit within the case.

The following image shows adjusted pin headers on the left and the original position of the plastic spacer on the right.

<img src="/buildimages/v1.0/sunrise-step3-parts.jpg" style="width:auto" height="154" alt="Parts required for step 2 of assembly"/>



<ol>
<li>Orientate the PCB so that the 8 way right angle PIN header is underneith and on the right hand thin side. 
<br/>
The PCB socket attached in the previous step will be on the side facing upwards.</li>
<li>
Solder the 5 way pin header on the left hand (thin) side with one hole separating it from the bottom of the PCB.
</li>
<li>
Solder the 4 way pin header 13 holes from the left hand (thin) side with two holes separating it from the bottom of the PCB.
</li>
</ol>

The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step3-output.jpg" style="width:auto" height="200" alt="PCB after step 2 has been completed"/>

### Step 4 - Attach Sunrise CO2 Sensor

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|006-0-0007|Senseair Sunrise CO2 sensor|

Place the Senseair Sunrise CO2 sensor on the pins attached in the previous step. The pins must align exactly with the Senseair Sunrise PCB if they don't the previous step was not completed correctly.

<img src="/buildimages/v1.0/sunrise-step4-parts.jpg" style="width:auto" height="154" alt="Parts required for step 2 of assembly"/>

Solder each of the pin headers to the Senseair Sunrise sensor PCB. The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step4-output.jpg" style="width:auto" height="154" alt="PCB after step 2 has been completed"/>

### Step 4 - Attach Sunrise CO2 Sensor

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|006-0-0007|Senseair Sunrise CO2 sensor|

Place the Senseair Sunrise CO2 sensor on the pins attached in the previous step. The pins must align exactly with the Senseair Sunrise PCB if they don't the previous step was not completed correctly.

<img src="/buildimages/v1.0/sunrise-step4-parts.jpg" style="width:auto" height="154" alt="Parts required for step 2 of assembly"/>

Solder each of the pin headers to the Senseair Sunrise sensor PCB. The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step4-output.jpg" style="width:auto" height="154" alt="PCB after step 2 has been completed"/>


### Step 5 - Wire 3.3V VIN (Red wire)

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|Wire|Red wire|

Place the PCB so that the CO2 sensor & BME280 socket are on the side facing upwards. Orienate it so that the BME280 socket is on the bottom side and the 8way header pins are on the left (actual pin connectors on the underside).

Solder a piece of red wire to pin 2 on the 8 way right angle connector whos pins are on the right hand side. See image below.

<img src="/buildimages/v1.0/sunrise-step5-a.jpg" style="width:auto" height="200" alt="Connection from pin 2 of 8 way for VIN"/>

Cut the wire and orientate it in the manner shown in the image below. The end of the wire should be stripped to a length which allows it to pass through the hole above the left hole on the BME280 socket and touch the left BME280 socket pin on the otherside of the PCB.

<img src="/buildimages/v1.0/sunrise-step5-b.jpg" style="width:auto" height="200" alt="Connection from pin 2 of 8 way to hole beside BME280 VIN pin with wire pushed through hole"/>

Turn the PCB over and ensure the BME280 socket pins are on the bottom side. The 8 way right angle connector will be on the left hand side.

Attach a piece of red wire to the two pins three up from the bottom of the PCB on the far right hand side. See the image below.

<img src="/buildimages/v1.0/sunrise-step5-c.jpg" style="width:auto" height="154" alt="Connection from pin 2 of 8 way to hole beside BME280 VIN pin with wire pushed through hole"/>

Shorten and strip the wire so that it can connect with the wire coming from the other side of board and the right hand BME280 socket pin.

Solder the pin and the two wires together. The result should look similar to the image below.

<img src="/buildimages/v1.0/sunrise-step5-d.jpg" style="width:auto" height="154" alt="Connection from pin 2 of 8 way to hole beside BME280 VIN pin with wire pushed through hole"/>


### Step 6 - Wire GND (Black wire)

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|Wire|Black wire|

Place the PCB so that the CO2 sensor & BME280 socket are on the side facing upwards. Orienate it so that the BME280 socket is on the bottom side and the 8way header pins are on the left (actual pin connectors on the underside).

Solder a piece of black wire to pin 1 on the 8 way right angle connector who's pins are on the right hand side. This wire should be the right length to neatly go through the PCB next to the VIN connection.

Again leave enough stripped wire to touch the GND pin on the BME280 socket. See image below.

<img src="/buildimages/v1.0/sunrise-step6-a.jpg" style="width:auto" height="154" alt="Connection from pin 1 of 8 way for GND"/>

Turn the PCB so that the right angle pins are on top and the CO2 sensor is on the bottom.

Solder two lengths of cable onto the GND and COMSEL pins of the Senseair Sunrise sensor. The GND pin will require a longer length than the COMSEL pin.  See image below:-

<img src="/buildimages/v1.0/sunrise-step6-b.jpg" style="width:auto" height="154" alt="Two lengths of cable soldered onto the GND and COMSEL pins of the Senseair Sunrise sensor"/>

Shorten and strip the two lengths of wire just soldered so that they neatly reach the GND pin of the BME280 socket and GND wire coming from other side of the PCB.

Solder the two pieces of wire, the BME280 GND pin and the GND wire from the other side of the PCB together. See image below:-

<img src="/buildimages/v1.0/sunrise-step6-c.jpg" style="width:auto" height="154" alt="All GND wires soldered together"/>

### Step 7 - Wire I2C (Green and Blue wire)

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|Wire|Green & Blue wire|

The two colors of wire have the following meanings.

|Color|Purpose|
|--|--|
|Blue|I2C SDA|
|Green|I2C SCL|


Place the PCB so that the CO2 sensor & BME280 socket are on the side facing upwards. Orienate it so that the BME280 socket is on the bottom side and the 8way header pins are on the left (actual pin connectors on the underside).

Solder a length of blue wire (I2C SDA) to pin 3 on the 8 way right angle connector. Then solder a length of green wire (I2C SCL) to pin 4 on the same connector.

Adjust the length on each wire so that they both go through to the other side of the PCB at a location where there is space to connect wires on the other side.

Finally place a length of blue wire (I2C SDA) to connect from the blue "junction point" back to the BME280 socket SDA pin. This will be soldered from the other side of the board.

<img src="/buildimages/v1.0/sunrise-step7-a.jpg" style="width:auto" height="200" alt="I2C connections on sensor side of PCB."/>

Turn the PCB so that the right angle pins are on top and the CO2 sensor is on the bottom.

Solder the blue (I2C SDA) wire connections together and add an additional piece of blue wire to connect the Senseair Sunrise I2C pin. 

Solder the blue (I2C SDA) wire to the BME280 socket SDA pin. 

Solder the green (I2C SCL) wire connections together and route an additional green wire to both the BME280 socket SCL pin and the Senseair Sunrise socket pin. 

See image below:-

<img src="/buildimages/v1.0/sunrise-step7-b.jpg" style="width:auto" height="154" alt="I2C connections on pin connector side of PCB."/>

### Step 8 - Wire CO2 sensor control (White and yellow wire)

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|Wire|White & Yellow wire|

The two colors of wire have the following meanings.

|Color|Purpose|
|--|--|
|White|Enable Sensor|
|Yellow|Reading Ready|


Place the PCB so that the CO2 sensor & BME280 socket are on the side facing upwards. Orienate it so that the BME280 socket is on the bottom side and the 8way header pins are on the left (actual pin connectors on the underside).

Solder a length of white wire (Enable sensor) to pin 7 on the 8 way right angle connector. Then solder a length of yellow wire (Reading ready) to pin 8 on the same connector.

The white enable sensor wire should be adjusted so that it fits neatly to go through the PCB hole next to the Senseair Sunrise EN pin. Solder to connect to the EN pin on the other side of the PCB.

The yellow reading ready wire should be adjusted so that it fits neatly to go through the PCB hole next to the Senseair Sunrise nRDY pin. Solder to connect to the nRDY pin on the other side of the PCB.

<img src="/buildimages/v1.0/sunrise-step8-a.jpg" style="width:auto" height="154" alt="I2C connections on sensor side of PCB."/>

Finally place a BME280 breakout board into the socket. See image below:-
<img src="/buildimages/v1.0/sunrise-step8-b.jpg" style="width:auto" height="154" alt="I2C connections on pin connector side of PCB."/>

