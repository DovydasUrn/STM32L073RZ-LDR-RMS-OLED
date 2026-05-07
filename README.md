# STM32L073RZ-LDR-RMS-OLED

This repository contains an STM32 project for measuring an analog signal using the ADC, calculating RMS and amplitude values, reading two LDR light sensors, displaying results on an OLED screen, and sending data through UART.

## How to open the project

1. Download this repository as a ZIP file.
2. Extract the ZIP file.
3. Open STM32CubeMX.
4. Open the `.ioc` project file from the extracted folder.
5. Generate the code in STM32CubeMX.
6. Open the generated project in STM32CubeIDE.
7. Build and upload the project to the STM32 board.

## Main features

- ADC signal measurement
- RMS and amplitude calculation
- Two LDR light sensor inputs
- OLED display output
- UART data transmission

## Hardware used

- STM32L073RZ development board
- SSD1306 OLED display
- Two LDR sensors
- 10 kΩ resistors for LDR voltage dividers
- Breadboard and jumper wires

## Notes

The LDR sensors are connected as voltage dividers. Each LDR is connected to 3.3 V, the measurement point is connected to a separate ADC input, and a 10 kΩ resistor is connected from the measurement point to GND.

The measured LDR values are approximate because LDR sensors are not precision light measurement devices. Calibration may be required for more accurate lux values.
