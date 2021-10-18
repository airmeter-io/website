---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
maintitle: Home 
sortOrder: 1
permalink: /
breadcrumb:
    - 
      name: Home
---

![Landing screen in Web UI](https://i.ibb.co/py3drYb/ss1.png)
# What is AirMeter.io?

AirMeter.io is an Opensource platform that facilitates building Internet of Things (IoT) enabled CO2 monitoring devices. It has:
- A modern responsive Web UI.
- Calibration & configuration workflows.
- On device data logging & charting.
- Remote data logging to MQTT servers (e.g. "the cloud").
- A set of REST APIs.


The Web UI is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and simply invokes the REST APIs made available by the firmware. As the packaged ReactJS app is served from a dedicated partition by the C++ core of the firmware, it can be replaced entirely.

Presently AirMeter.io supports CO2 sensors listed below:
- [*Senseair*](https://senseair.com) - Senseair Sunrise (UART or I2C).
- [*Cubic Sensor*](https://www.en.gassensor.com.cn) - CM1107 & CM1106 (UART).
- [*Winsen*](https://www.winsen-sensor.com) - MH-Z19B, MH-Z19C, MH-Z14.




# Why Measure CO2?

The COVID-19 pandemic has brought an urgent requirement to measure CO2 to assess the performance and adequacy of ventilation.