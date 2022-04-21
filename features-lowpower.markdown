---
layout: default
sortOrder: 3
permalink: /features/lowpower
title: Low Power Operation
breadcrumb:
    - 
      name: Features
      url: /features
    - 
      name: Low Power Operation
---
*AirMeter.io* has been optimised for low power battery operation using power profiling equipment to achieve extremely low power consumption on the ESP32 family of microcontrollers. 

### Sensor Optimisations
Advanced low power CO2 sensors generally support a sequence along the lines of 
- Enable
- Wait
- Read
- Disable

This has been implemented for the Senseair Sunrise sensor and will also been included in the integration of any additional sensor families which support this feature.

### Connected To Wifi
In many cases *AirMeter.io* is intended to be used connected to a wireless network. Therefore by using a *Nordic Power Profiler Kit II* and leveraging some advanced ESP32 platform features a power draw of 5mA has been achieved in this mode.

Tests were performed using a LilyGo 2.13 ePaper Display ESP32 board. The readings and contents of the ePaper display updated once a minute.

These results translate to 15 days of runtime whilst fully connected to wifi and updating readings using a 1800mAh battery. 

### Disconnected Mode (Planned)
When using very low power sensors whilst the device is connected to wifi most of the power usage is maintaining that connection. 

Therefore a "disconnected mode" for when the device is away from or does not require connectivity will allow for substantially longer periods without a charge.

This mode will be able to utilise other power management features such as deep sleep since connections do not need to be maintained.


### Remote Monitoring Mode (Planned)
This is an extension of disconnected mode where the device is being used in a remote monitoring/data collection scenario with centralised logging via MQTT.

In this mode the device will wake up on a scheduled interval, connect to wifi and publish readings that have been taken.


