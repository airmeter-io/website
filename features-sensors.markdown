---
layout: default
sortOrder: 3
permalink: /features/sensors
title: Sensors
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Sensors     
---

There is support for multiple families of CO2 sensor. At present this include SenseAir, Cubic & Winsen sensors. Additional Sensor drivers will continue to be added on an ongoing basis.

The support for each sensor has been developed with care and in respect to the manufactures recommendations as far as is possible. Each sensor "driver" exposes functions which the UI layers use to configure and control the sensor. 

Presently AirMeter.io supports:
- [*Senseair*](https://senseair.com) - Senseair Sunrise (UART or I2C).
- [*Cubic Sensor*](https://www.en.gassensor.com.cn) - CM1107 & CM1106 (UART).
- [*Sensirion (PLANNED)*](https://www.sensirion.com/en) - SCD30.
- [*Winsen*](https://www.winsen-sensor.com) - MH-Z19B, MH-Z19C, MH-Z14.