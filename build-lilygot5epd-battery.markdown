---
layout: default
title: Prepare LiPO battery
permalink: /make/epd213/battery
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ePaper Display
      url: /make/epd213   
    - 
      name: Prepare LiPO Battery
---

The [LILYGO® TTGO T5 board](/make/epd213/prepare) uses a 1.25mm pitch JST connector for the battery. Any battery compatible with the [LILYGO® TTGO T5 board](/make/epd213/prepare) should work. 

However understand that this design has been dimensioned on the assumption that the battery is a FT103450P. If a battery of different dimension is used the [3D models](/make/epd213/assemble) may need to be adjusted to accomodate it's dimensions.

## Attaching 1.25mm JST connector

Get the following parts ready before starting this step.

|Part|Description|
|--|--|
|1.25mm JST connector|Each [LILYGO® TTGO T5 board](/make/epd213/prepare) board is shipped with a suitable JST connector wire. If using a third party item please ensure the polarity and size are correct|
|FT103450P|A 1800mAh lipo battery|

The 1.25mm JST connector lead needs to be solidered to the battery wires matching the colors on both sides. Alternatively if you have the correct tools a JST connector maybe crimped directly onto the battery wires.

Ensure there is around 10cm of wire available. This is more than enough however leaving some wire at each end can be useful in future.


<img src="/buildimages/v1.0/battery.jpg" style="width:auto" height="200" alt="Battery with 1.25mm JST connector attached."/>

When sure the battery is soldered solidly one must use insulation tape (or a suitable alternative) to ensure that no short circuits can occur between the wires. 

It seems to be better to apply tape separately on the GND and VIN wires. This gives more flexibility routing the wires when [assembling](/make/epd213/assemble).

