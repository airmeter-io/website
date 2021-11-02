---
layout: default
sortOrder: 3
permalink: /features/logging
title: Data Logging
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Data Logging
---
Up to six months of readings can be recorded in flash memory. The readings can be viewed within the Web UI using the charts screen. 

AirMeter.io is intended to be used as a data logger. On a standard configuration device six months of readings every minute for temperature, pressure, humidity & time of reading can be stored on a flash partition.

These readings can be view using a [Charts.js](https://www.chartjs.org/) show values over time in the web interface. The results can (*planned functionality*) by downloaded as XML, JSON or CSV.

This data logging function and UI to view relies sole on the device itself so can be used in disconnected environments or cases where there are not enough devices to warrant centralised logging and monitoring.

Data logging does rely on NTP time synchronisation to ensure the datapoints are correctly timestamped.