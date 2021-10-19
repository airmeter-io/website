---
layout: default
sortOrder: 3
permalink: /features/lowpower
title: Low Power (Planned)
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Low Power (Planned)
---

The planned low power mode will take a number of steps to minimise power consumption:
- If supported utilise CO2 sensor in "single measurement mode" therefore powering off sensor when not in use.
- Put BME280/BMP280 sensor into sleep mode after reading.
- Put microcontroller into deep sleep until next reading, next MQTT publish or a nominated GPIO is triggered.
- Utilise RTC memory where appropriate.
- Method and fine tuning of same to enable Wifi. Probably via menu on screen, automatically when USB connected & possibly key press sequence for screenless devices.