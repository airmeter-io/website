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

# What is AirMeter.io?
AirMeter.io is an Opensource platform that facilitates building Internet of Things (IoT) enabled CO2 monitoring devices. 

![Landing screen in Web UI](https://i.ibb.co/D9CSpRw/banner.png)

It has a modern responsive Web UI with built in calibration & configuration workflows. The on device data logging & charting features allow the monitor to operate indepenantly. Equally an AirMeter.io device can be used as part of a cloud using its MQTT publishing features.

The Web UI is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and simply invokes REST APIs made available by the firmware. As the packaged ReactJS app is served from a dedicated partition by the C++ core of the firmware, it can be replaced entirely.





# Why Measure CO2?

The COVID-19 pandemic has brought an urgent requirement to measure CO2 to assess the performance and adequacy of ventilation.