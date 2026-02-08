# ESPhome Multisensor

This project is a compact ESPhome-compatible multisensor shield. The PCB is designed so that all required components can be hand-soldered—no SMD reflow oven or pick-and-place machine is required.

The shield is modular and prepared for multiple purposes. The primary use case is as an ESPHome sensor with multiple sensor values available:

## Features

- Measuring temperature and humidity with the onboard SHT40 I2C sensor
- Measuring brightness with PT19-21C
- Detecting human presence with LD2410B mmWave sensor
- Detecting motion with PIR sensor SR602
- 2x Onboard WS2812B LEDs For addressable color light
- SolidState Relais TLP175A for poential free contact
- Solder connections for several sensor modules like
  - BME280 -> temperature and humidity and air pressure
  - SCD40 -> CO2, temperature and humidity
  - SHT40 -> temperature and humidity
  - and many others
- QWIIC connector for connecting additional QWIIC-compatible modules if needed

The idea is to have one general-purpose PCB and only populate the components necessary for your use case.

For example, if you want to use a SCD40 sensor to measure the CO2 level in a room, you don't need the onboard SHT40 sensor since the SCD40 already provides temperature and humidity data.

Images:

![Schematic](assets/schematic.svg)

![Top view](assets/board_3d.png)

Notes:
- Gerber files available from the Actions. [![Generate Fabrication Files](https://github.com/ThomasLindenberger37/ESP32_Sheald/actions/workflows/fabrication.yml/badge.svg)](https://github.com/ThomasLindenberger37/ESP32_Sheald/actions/workflows/fabrication.yml)
