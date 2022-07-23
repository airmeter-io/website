---
layout: default
title: Prepare LiPO battery
permalink: /make/epd213/battery
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ePaper
      url: /make/epd213   
    - 
      name: Prepare LiPO Battery
---

The LILYGO® TTGO T5 V2.3.1_2.13 board uses a 1.25mm pitch JST connector for the battery. 

Any battery compatible with the TTGO board should work. However understand that this design has been dimensioned on the assumption that the battery is a FT103450P. If a battery of different dimension is used the 3D models may need to be adjusted.

## Instructions

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|1.25mm JST connector|Each LILYGO® TTGO T5 V2.3.1_2.13 board is shipped with a suitable connector wire. If using a third party item please ensure the polarity and size are correct|
|FT103450P|A 1800mAh lipo battery|

The 1.25mm JST connector lead needs to be attached to the battery matching the colors on both sides. If you have the tools to crimp a connector then you may do this instead.

Ensure there is around 10cm of wire available. This is more than enough however leaving some wire at each end can be useful if needing to repair.

<img src="/buildimages/v1.0/battery.jpg" style="width:auto" height="200" alt="Battery with 1.25mm JST connector attached."/>

When sure the battery is soldered solidly one must use insulation tape (or alternative) to ensure that no short circuits occur between the two poles. 

It seems to be better to apply tape separately on the GND and VIN wires, as this gives more flexibility when assembling without crushing wires.

