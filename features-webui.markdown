---
layout: default
sortOrder: 3
permalink: /features/webui
title: Responsive Web UI
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Responsive Web UI 
---

The Web UI is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and invokes the [REST APIs made available](/api) by the firmware. As the packaged ReactJS app is served from a dedicated partition by the C++ core of the firmware, it can in-fact be replaced entirely.

The available REST APIs are documented [here](/api). These APIs allow full customisation of the Web UI, centralised and automated control of devices using the AirMeter.io firmware.