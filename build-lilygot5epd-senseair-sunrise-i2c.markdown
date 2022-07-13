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

## Overview

This page describes how to build the Sensor Assembly for a Senseair Sunrise CO2 sensor. This board connects to a LilyGO 2.13in EPD displayboard via a right angle pin header mounted on the board.

Once completed this part will appear in as shown in the image below.
<img src="/buildimages/v1.0/sunrise-finished-top.jpg" style="width:auto" height="324" alt="Completed Sensor Assembly for a Senseair Sunrise CO2 sensor"/>



## Parts

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

## Wire Colors

|Color|Purpose|
|--|--|
|Black|Ground|
|Red|3.3v|
|Blue|I2C SDA|
|Green|I2C CLK|
|White|Reading Ready|
|Yellow|Enable Sensor|


## Build Steps 

### Step 1 - Attach the 8 way right angle pin header

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|2.54mm pin header|8 Way, 1 row, right angle pin header|

<img src="/buildimages/v1.0/sunrise-step1-parts.jpg" style="width:auto" height="400" alt="Parts required for step 1 of assembly"/>

At one thin (10 holes/3cm wide) end of the PCB attach the pin header to the PCB using solder. The pins must face inwards towards the other thin end of the PCB. 

After completing this step the PCB should appear as in the the image below.

<img src="/buildimages/v1.0/sunrise-step1-output.jpg" style="width:auto" height="400" alt="PCB after step 1 has been completed"/>


### Step 2 - Attach 4 way PCB Socket for BME280 board

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|2.54mm socket|4 Way 1 Row Straight PCB Socket Through Hole|


<img src="/buildimages/v1.0/sunrise-step2-parts.jpg" style="width:auto" height="354" alt="Parts required for step 2 of assembly"/>

<ol>
<li>Orientate the PCB so that the PIN header is underneith and on the right hand side. </li>

<li>At the bottom and six holes in from the right of the PCB mount the 4 way socket using solder.</li>
</ol>

The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step2-output.jpg" style="width:auto" height="400" alt="PCB after step 2 has been completed"/>

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

<img src="/buildimages/v1.0/sunrise-step3-parts.jpg" style="width:auto" height="354" alt="Parts required for step 2 of assembly"/>



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

<img src="/buildimages/v1.0/sunrise-step3-output.jpg" style="width:auto" height="400" alt="PCB after step 2 has been completed"/>

### Step 4 - Attach Sunrise CO2 Sensor

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|006-0-0007|Senseair Sunrise CO2 sensor|

Place the Senseair Sunrise CO2 sensor on the pins attached in the previous step. The pins must align exactly with the Senseair Sunrise PCB if they don't the previous step was not completed correctly.

<img src="/buildimages/v1.0/sunrise-step4-parts.jpg" style="width:auto" height="354" alt="Parts required for step 2 of assembly"/>

Solder each of the pin headers to the Senseair Sunrise sensor PCB. The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step4-output.jpg" style="width:auto" height="400" alt="PCB after step 2 has been completed"/>

### Step 4 - Attach Sunrise CO2 Sensor

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|006-0-0007|Senseair Sunrise CO2 sensor|

Place the Senseair Sunrise CO2 sensor on the pins attached in the previous step. The pins must align exactly with the Senseair Sunrise PCB if they don't the previous step was not completed correctly.

<img src="/buildimages/v1.0/sunrise-step4-parts.jpg" style="width:auto" height="354" alt="Parts required for step 2 of assembly"/>

Solder each of the pin headers to the Senseair Sunrise sensor PCB. The PCB will appear as shown in the image below when this step is completed.

<img src="/buildimages/v1.0/sunrise-step4-output.jpg" style="width:auto" height="400" alt="PCB after step 2 has been completed"/>


### Step 5 - Wire 3.3V VIN (Red wire)

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|22402A-17|3cm x 7cm double sided universal PCB|
|Wire|Red wire|

Place the PCB so that the CO2 sensor & BME280 socket are on the side facing upwards. Orienate it so that the BME280 socket is on the bottom side and the 8way header pins are on the left (actual pin connectors on the underside).

Solder a piece of red wire to pin 2 on the 8 way right angle connector whos pins are on the right hand side. See image below.
<img src="/buildimages/v1.0/sunrise-step5-a.jpg" style="width:auto" height="354" alt="Connection from pin 2 of 8 way for VIN"/>

Cut the wire and orientate it in the manner shown in the image below. The end of the wire should be stripped to a length which allows it to pass through the hole above the left hole on the BME280 socket and touch the left BME280 socket pin on the otherside of the PCB.

<img src="/buildimages/v1.0/sunrise-step5-b.jpg" style="width:auto" height="354" alt="Connection from pin 2 of 8 way to hole beside BME280 VIN pin with wire pushed through hole"/>

Turn the PCB over and ensure the BME280 socket pins are on the bottom side. The 8 way right angle connector will be on the left hand side.

Attach a piece of red wire to the two pins three up from the bottom of the PCB on the far right hand side. See the image below.

<img src="/buildimages/v1.0/sunrise-step5-c.jpg" style="width:auto" height="354" alt="Connection from pin 2 of 8 way to hole beside BME280 VIN pin with wire pushed through hole"/>

Shorten and strip the wire so that it can connect with the wire coming from the other side of board and the right hand BME280 socket pin.

Solder the pin and the two wires together. The result should look similar to the image below.

<img src="/buildimages/v1.0/sunrise-step5-d.jpg" style="width:auto" height="354" alt="Connection from pin 2 of 8 way to hole beside BME280 VIN pin with wire pushed through hole"/>


