---
layout: default
title: Parts
permalink: /make/esp32/parts
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ESP32
      url: /make/esp32
    -
      name: Parts
---

# ESP32 Family Microcontroller

The requirement is an ESP32 Family Microcontroller with at least 4 megabytes of flash memory. The microcontroller can be any of the following:
- EP32
- ESP32-S2
- ESP32-C3 
- ESP32-S3
- ESP32-C6

The breadboard development assembly instructions are written from the assumption that an ESP32-WROOM-32 board is being used.

# Pressure, temperature and humidity sensor

The supported sensors at this time are:
- Bosch BME280
- Bosch BMP280

These sensors provides temperature, pressure and humidity readings. It can be substituted with a GY-BMP280 if required. The BME280 is presently in short supply.

# Display

The supported display is an SSD1306 connected via I2C. 

*Support for ST7735 & ST7789 is planned as a priority*

The display is used to enable secure WiFi provisioning and to display live readings. 

# CO2 Sensor

## Senseair Sunrise

The Senseair Sunrise is an excellent sensor and has been a primary focus of testing and development due to its recognised use is premium commercial devices.

This sensor can be connected either via I2C or UART. At present the UART implementation is considered most stable and should be preferred. 


## Cubic CM1107/CM1106

Cubic are reported to produce high quality sensors and AirNeter.io has full support for these sensors. However as all testing has been performed on second hand units AirMeter.io, it is impossible to comment further.


## Winsen MH-Z19B/C & MH-Z14

The Winsen MH-Z19B/C sensors are fully supported and tested "functionally". Results may vary but it is worth noting that:
- These sensors generally require forced background calibration.
- Voltage and quality of power supply maybe important.

The MH-Z14 sensor has been lightly tested but has not been deeply investigated and tested.

# FRAM datalogging storage (Optional)
An FRAM module for persistent data staging before writing to flash can be included connected to the I2C bus. Without this component any data that is not written to the flash will be lost. To prevent undue wear on the flash the firmware has to wait until there are quite a number of readings waiting to be written.

For builds where data logging is important this is an essential component.

# Enclosure and Electrical Connections
Breadboards are useful for experimental builds. An alternative such as soldering to a PCB or just jumper leads is also effective and more appropriate for long term use devices.

However for simplicity the assembly instructions assume breadboard are being used. Each build requires two mini-breadboards to be able to access all the relevant pins on the components.


