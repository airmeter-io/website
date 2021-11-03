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
Full support for effective low power usage is planned for ESP32 family devices.

### Initial Platform
Initially the LilyGo 2.13 ESP32 ePaper board will be used as the development platform for the low power profile.

### Sensor Optimisations
If supported utilise CO2 sensor in "single measurement mode" therefore powering off sensor when not in use. The BME280/BMP280 sensors support sleep mode which will be utilised.


### ESP32 Platform Optimisations
An option will be added to put  microcontroller into deep sleep between readings, next MQTT publish or a nominated GPIO is triggered. Actions such as connecting & disconnecting a power source will be able to trigger enabling/disabling the web interface.

A combination of RTC memory, wake stubs and ULP will be utilised to achieve low power operation.

The user experience will be considered and introduction of on-device menuing using the connected display is essential in providing a quality experience.
