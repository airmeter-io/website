---
layout: default
sortOrder: 3
permalink: /features/datalogging
title: Data Logging
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Data Logging
---

Up to six months of readings can be recorded in flash memory. The readings can be viewed within the web interface using the charts screen. 

AirMeter.io is intended to be used as a data logger. Generally up to six months of readings (once every minute including temperature, pressure, humidity & time) can be stored on the device's flash memory.

### Charting
These readings can be viewed using a [Charts.js](https://www.chartjs.org/) show values over time in the web interface. The results can (*planned functionality*) by downloaded as XML, JSON or CSV.


### No internet or infrastructure required
This data logging function and UI to view relies sole on the device itself so can be used in disconnected environments or cases where there are not enough devices to warrant centralised logging and monitoring.


### NTP time synchronisation
Data logging does rely on NTP time synchronisation to ensure the datapoints are correctly timestamped.