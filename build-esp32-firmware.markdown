---
layout: default
title: Firmware Build Instructions
permalink: /make/esp32/firmware_build
breadcrumb:
    - 
      name: Make a Device
      url: /make
    - 
      name: ESP32
      url: /make/esp32
    -
      name: Firmware Build Instructions
---

When the AirMeter.io firmware is built for the ESP32 platform it uses the latest v4.3 ESP32 IDF SDK. 


## Windows Environment Setup

Espressif provide a Windows package which ensures all the required components are installed. This is the easist way to setup a Windows build environment, the install can be found at [https://dl.espressif.com/dl/esp-idf/?idf=4.4](https://dl.espressif.com/dl/esp-idf/?idf=4.4). Install the v4.3 sdk.

More indepth instructions and alternative manual installation methods can be found at [https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/windows-setup.html](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/windows-setup.html).

The remaining instructions in this document assume that the "ESP-IDF CMD" link on the start menu is being used as the CLI to enter commands.

## Linux Environment Setup

Follow the instructions at [https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/) and ensure that the user enviroment is set up correctly.

The remaining instructions in this document assume that the users shell has the appropriate enviroment variables set and the IDF v4.3 SDK checked out.
  

## Clone & initialise the latest AirMeter.IO Monitor firmware


Clone the repository & change into the directory.

    git clone https://github.com/airmeter-io/AirMeter.IO.Firmware.git
    cd AirMeter.IO.Firmware

  
Initialise  the GIT Submodules.

    git submodule init
    git submodule update

Copy the ESP32 SDK config files to the project root director.

On Linux type:-

    cp boards/esp32-idf/sdkconfig* .


On Windows type:-

    copy boards\esp32-idf\sdkconfig*.* .




## Build the project

Type the following to build the project.

    idf.py build


  
## Flash to device

On Linux type:

    idf.py flash /dev/ttsyusb0

Replace /dev/ttsyusb0 with the com port device exposed by the ESP32-WROOM32 board.

On Windows type:

    idf.py flash COM4

Replace COM4 with the correct COM port exposed by the ESP32-WROOM32 board.


