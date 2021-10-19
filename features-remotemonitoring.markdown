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

Readings can be published using MQTT to either third-party cloud services or to a server setup to be a dedicated "private/local cloud". MQTT is supported due to its prevalence. Other protocols for publishing readings may be added in future if they would serve a user base.

The frequency of publishing to the MQTT server can be altered and may be different from the frequency of reading sensor values & writing to the on-device data log.

This feature relies on NTP time synchronisation to ensure the datapoints are correctly timestamped.