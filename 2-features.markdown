---
layout: default
title: Features & Hardware
maintitle: Features
permalink: /features/
sortOrder: 2
breadcrumb:
    - 
      name: Features
      
---

The AirMeter.io firmware has a rich feature set to which more is being added regularly. Below you will find a summary of the most important and links to pages describing the features in detail.

### [CO2 Sensor Families](/features/sensors)
There is support for multiple families of CO2 sensor. At present this include *SenseAir*, *Cubic* & *Winsen* sensors. Additional drivers for different manufactures and models can be added without difficulty assuming the ICs are available to test.

### [Responsive Web Interface](/features/webui)
The web interface is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and simply invokes REST APIs made exposed by the firmware. As the packaged ReactJS app is served from a dedicated partition by the C++ core, it can be replaced entirely with any application written in JavaScript.

### [Calibration](/features/calibration) 
Calibration is very important to maintain accuracy. *AirMeter.io* makes the process of forcing background calibration and configuring ABC (Automatic Background Calibration) a breeze. Wizards are provided to guide users through the required steps.

### [Device Configuration](/features/configuration)
All settings including wireless, NTP and data logging can be managed through the Web UI. They can also be set by calling the REST APIs directly.

### [Captive Portal](/features/captiveportal) 
By default a device boots and starts an access point with a captive portal secured using WPA2 to allow the device to be configured.

### [Data Logging and Charting](/features/datalogging)
Up to six months of readings can be recorded in flash memory. The readings can be viewed within the web interface using the charts screen. 

### [Remote Monitoring](/features/remotemonitoring) 
*AirMeter.io* device can be used as part of a cloud using the MQTT publishing feature. The frequency and target MQTT server are configurable through the Web UI and directly using the REST APIs.

### [Low Power Mode (Planned)](/features/lowpower)
Full support for effective low power usage is planned. The initial implementation will be based upon the LilyGo 2.13 ESP32 ePaper board.

### [Hardware](/features/hardware) 
ESP32 & ESP8266 family MCUs made by Espressif can be used as the platform on which the build a device. Both chip families have a wide range of boards available in different form factors and bundled peripheral components.