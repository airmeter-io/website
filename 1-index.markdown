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

It has a modern responsive Web UI with built in calibration & configuration workflows. The on-device data logging & charting features allow the monitor to operate independently. Equally an AirMeter.io device can be used as part of a cloud using its MQTT publishing features.

The Web UI is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and simply invokes REST APIs made available by the firmware. As the packaged ReactJS app is served from a dedicated partition by the C++ core of the firmware, it can be replaced entirely.


# Why Measure CO2?

It is now accepted by major public health agencies that COVID-19 can and does spread through aerosols. See [Centers for Disease Control and Prevention](https://www.cdc.gov/coronavirus/2019-ncov/science/science-briefs/sars-cov-2-transmission.html), [World Health Organisation (WHO)](https://www.who.int/news-room/q-a-detail/coronavirus-disease-covid-19-how-is-it-transmitted), [European Centre for Disease Prevention and Control (ECDC)](https://www.ecdc.europa.eu/en/covid-19/questions-answers/questions-answers-basic-facts).

The outside CO2 level away from combustion sources is relatively constant at ~415ppm. When a person exhales the release air containing 35,000-45,000ppm therefore the level of CO2 in an enclosed space is a *proxy* to the level of exhaled air which hasn't been ventilated.

If the CO2 level is too high then ventilation & filtration are the primary approaches to reducing the level of potentially dangerous aerosols. 

