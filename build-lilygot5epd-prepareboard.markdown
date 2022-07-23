---
layout: default
title: Prepare LilyGo board
permalink: /make/lilygo213/prepare
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: LilyGO 2.13in EPD
      url: /make/lilygo213   
    - 
      name: Prepare board
---

## Parts

|Part|Description|
|--|--|
|LILYGO® TTGO T5 V2.3.1_2.13|2.13in EPD and ESP32 board with battery charging support.  DEPG0213BN version is supported currently. |
|2.54mm pin socket|8 Way, 1 row, socket|
|Wire|Six colors of wire.|

## Wire Colors

|Color|Purpose|
|--|--|
|Black|Ground|
|Red|3.3v|
|Blue|I2C SDA|
|Green|I2C SCL|
|White|Enable Sensor|
|Yellow|Reading Ready|



## Build Steps 

### Step 1 - Attach 6 lengths of wire.

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|LILYGO® TTGO T5 V2.3.1_2.13|2.13in EPD and ESP32 board with battery charging support.  DEPG0213BN version is supported currently. |
|Wire|Six colors of wire.|

The lengths of wire should be attached to the following pins.

|Color|Purpose|LilyGO Pin|
|--|--|--|
|Black|Ground|GND|
|Red|3.3v|3.3|
|Blue|I2C SDA|21|
|Green|I2C SCL|22|
|White|Enable Sensor|19|
|Yellow|Reading Ready|15|

Enough wire must be left to complete the following steps. See image below:-

<img src="/buildimages/v1.0/lilygo213-step1.jpg" style="width:auto" height="200" alt="LilyGo board with 6 lengths of wire attached."/>


### Step 2 - Route & bundle wires

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|LILYGO® TTGO T5 V2.3.1_2.13|2.13in EPD and ESP32 board with battery charging support.  DEPG0213BN version is supported currently. |

Route the wires towards the end of the LilyGo board opposite the buttons and USB ports. Create bends and use tape to secure the wires as a neat bundle.

See image below for desired result:-


<img src="/buildimages/v1.0/lilygo213-step2.jpg" style="width:auto" height="200" alt="LilyGo board with 6 lengths of wire routed and bundled together."/>

### Step 2 - Solder 8 way socket

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|LILYGO® TTGO T5 V2.3.1_2.13|2.13in EPD and ESP32 board with battery charging support.  DEPG0213BN version is supported currently. |


The objective of this step is to connect each of the wires to the appropriate pin on the 8 way socket. This socket will attach to the 8 way header on the base of the sensor assembly.

The pin connections must be as follows:-

|Color|Purpose|Socket PIN|
|--|--|--|
|Black|Ground|1|
|Red|3.3v|2|
|Blue|I2C SDA|3|
|Green|I2C SCL|4|
|White|Enable Sensor|7|
|Yellow|Reading Ready|8|


Clearly the aim here is to achieve enough slack to make assembly possible but also to avoid using excessive lengths of wire and damaging connections during assembly.

See image below for desired result:-


<img src="/buildimages/v1.0/lilygo213-step3.jpg" style="width:auto" height="200" alt="LilyGo board with 6 lengths of wire routed and bundled together."/>

