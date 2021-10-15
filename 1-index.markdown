---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
maintitle: Home 
sortOrder: 1
permalink: /
---


# What is AirMeter.io?

AirMeter.io is an Opensource platform that facilitates building Internet of Things (IoT) enabled CO2 monitoring devices. It is a customisable firmware that provides:
- A modern responsive Web UI.
- A set of REST APIs.
- On device data logging & charting.
- Remote data logging to MQTT servers (e.g. "the cloud").
- Calibration & configuration workflows.

The Web UI is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and simply invokes the REST APIs made available by the firmware. As the packaged ReactJS app is served from a dedicated partition by the C++ core of the firmware, it can be replaced entirely.

So far AirMeter.io supports CO2 sensors manufactured by SenseAir, Cubic & Winsen with more following in time. 

The firmware is built upon the [Espressif ESP-IDF SDK]() and [Espressif ESP-8266-RTOS SDK]() and therefore is designed to operate on the MCUs supported by these SDKs namely ESP32, ESP32-S2. ESP32-C3, ESP32-S3, ESP32-C6 & ESP8266. These SDKs were chosen due the popularity of these MCUs with makers and existing CO2 monitoring projects.

AirMeter.io is primarily about the Software & user experience. Reference designs are given as a starting point to makers but it is intended also to bring new features to existing designs & builds which satisfy the hardware requirements.

# Why Measure CO2?

The COVID-19 pandemic has brought an urgent requirement to measure CO2 to assess the performance and adequacy of ventilation.