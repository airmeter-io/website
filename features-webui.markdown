---
layout: default
sortOrder: 3
permalink: /features/webui
title: Responsive Web Interface
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Responsive Web Interface
---

The on-device web interface is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and simply invokes REST APIs made exposed by the firmware. 

### Customisable Web Interface
As the packaged ReactJS app is served from a dedicated partition by the C++ core, it can be replaced entirely with any application written in JavaScript that calls these REST APIs.

### REST API
The APIs themselves are documented [here](/api). They can also be used centralised automated control of AirMeter.io devices.