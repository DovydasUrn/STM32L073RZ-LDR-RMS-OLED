# STM32L073RZ-LDR-RMS-OLED
   
This repository contains an STM32 embedded systems project for analog signal measurement, light sensing, data processing, OLED display output, and UART data transmission to a computer.

## How to open the project

1. Download this repository as a ZIP file.
2. Extract the ZIP file.
3. Open STM32CubeMX.
4. Open the `.ioc` project file from the extracted folder.
5. Generate the code in STM32CubeMX.
6. Open the generated project in Keil uVision5.
7. Build and upload the project to the STM32 board.

The system measures:
- AC voltage using one ADC channel;
- light intensity using two LDR sensors;
- RMS and amplitude of the input signal;
- average and difference values of the two LDR channels.

## Project description

The project is based on the STM32L073RZ microcontroller.  
The microcontroller reads analog signals through its ADC inputs, processes the measured values in software, displays the results on an OLED screen, and sends the data to a computer using UART.

The AC voltage signal is measured through a voltage divider circuit. The measured ADC samples are used to calculate the RMS value and amplitude of the signal.

Two LDR sensors are used for light measurement. Each LDR is connected to a separate ADC input through a voltage divider circuit. The software converts the ADC values to approximate light intensity values and calculates the average and difference between the two LDR channels.

## Main features

- ADC-based analog signal measurement
- RMS value calculation
- Signal amplitude calculation
- Two-channel LDR light sensing
- LDR average and difference calculation
- OLED display output
- UART data transmission to PC

## Hardware used

- STM32L073RZ development board
- SSD1306 OLED display
- 2 × LDR light sensors
- Resistors for LDR voltage dividers
- MCP6002 operational amplifier
- Voltage divider resistors for AC signal measurement
- If needed use schottky diodes for input protection
- USB-UART converter
- Breadboard and jumper wires
- Function generator for testing
