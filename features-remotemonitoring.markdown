---
layout: default
sortOrder: 3
permalink: /features/remotemonitoring
title: Remote Monitoring
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Remote Monitoring    
---
AirMeter.io device can be used as part of a cloud using the MQTT publishing feature. The frequency and target MQTT server are configurable through the Web UI and directly using the REST APIs.

### MQTT
Readings can be published to either cloud services or to any MQTT server. For relative small setups a Raspberry PI4 with an SD card is more than sufficient.
 MQTT is supported due to its prevalence. 

Other messaging/publishing protocols may be added in future.

### Configuration and time sync
The frequency of publishing to the MQTT server is configurable and may differ from the sensor reading frequency. 

This feature relies on NTP time synchronisation to ensure the data points are timestamped correctly.