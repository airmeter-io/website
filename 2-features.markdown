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

# Support for Several CO2 Sensor Families

The support for each sensor has been developed with care and in respect to the manufacters recommendations as far as is possible. Each sensor "driver" exposes functions which the UI layers use to configure and control the sensor. 

Presently AirMeter.io supports:
- [*Senseair*](https://senseair.com) - Senseair Sunrise (UART or I2C).
- [*Cubic Sensor*](https://www.en.gassensor.com.cn) - CM1107 & CM1106 (UART).
- [*Sensirion (PLANNED)*](https://www.sensirion.com/en) - SCD30.
- [*Winsen*](https://www.winsen-sensor.com) - MH-Z19B, MH-Z19C, MH-Z14.

# Modern & Replacable Responsive WebUI

The Web UI is built using [ReactJS](https://reactjs.org), [Charts.js](https://www.chartjs.org/)  & [Canvas Gauges](https://canvas-gauges.com/) and invokes the [REST APIs made available](/api) by the firmware. As the packaged ReactJS app is served from a dedicated partition by the C++ core of the firmware, it can in-fact be replaced entirely.

The REST APIs are fully documented [here](/api). Apart from full customisation these APIs are also available for centralised and/or automated control of devices.

# Calibration & Configuration Workflows

The CO2 sensor needs to be recalibrated every now and then. The interval between calibrations depends on a number of factors:
- The sensor design and characteristics. Some sensors need to be calibrated more often than others.
- Whether the sensor receives shocks & wear/tear. Over time the bulb in a sensor can change in brightness and shocks can misalign components.
- General drift in readings the extent of this appears to be very sensor model dependent.

The AirMeter.io provides rich web wizard style workflows for managing calibration. These workflow will be replicated with the physical display/buttons in future development.


# Secure Captive Portal Onboarding Process





# Low Power Mode (Planned)

# Hardware 
The firmware is built upon the [Espressif ESP-IDF](https://github.com/espressif/esp-idf) and [Espressif ESP-8266-RTOS](https://github.com/espressif/ESP8266_RTOS_SDK) SDKs and therefore is designed to operate on the MCUs supported by these SDKs namely ESP32, ESP32-S2. ESP32-C3, ESP32-S3, ESP32-C6 & ESP8266. These SDKs were chosen due the popularity of these MCUs with makers and existing CO2 monitoring projects.

AirMeter.io is primarily about the Software & user experience. Reference designs are given as a starting point to makers but it is intended also to bring new features to existing designs & builds which satisfy the hardware requirements.
