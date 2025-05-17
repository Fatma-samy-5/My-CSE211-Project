# My-CSE211-Project
# Real-Time Clock and Analog Signal Display with Nucleo Board

![Project Demonstration](https://drive.google.com/file/d/1a5-6-lx1gGz0rocJ5X8RKrLVmOLAT9_K/view?usp=drivesdk)

## Project Overview
This project implements two main functionalities using a **Nucleo board** with an **Arduino multifunction shield**:
1. **Real-Time Clock (RTC)** - Displays elapsed time in MM:SS format
2. **Analog Signal Display** - Shows potentiometer voltage when activated

## Features
- 4-digit 7-segment display output
- Reset functionality with button S1
- Voltage monitoring via onboard potentiometer
- Toggle between time/voltage display with button S3
- Automatic min/max voltage tracking

## Hardware Requirements
- STM32 Nucleo board (any model)
- Arduino multifunction shield with:
  - 4-digit 7-segment display
  - 3 push buttons
  - Potentiometer
- USB cable for programming/power

## Pin Connections
| Shield Component | Nucleo Pin |
|-----------------|-----------|
| Shift Register Data | D8 |
| Shift Register Clock | D7 |
| Shift Register Latch | D4 |
| Button S1 (Reset) | A1 |
| Button S3 (Voltage) | A3 |
| Potentiometer | A0 |

## Software Requirements
- Mbed Studio or Mbed CLI
- Mbed OS 6.x
- STM32 HAL libraries

## How It Works
1. **On Startup**:
   - Clock begins counting from 00:00
   - Min/max voltage tracking initialized

2. **Normal Operation**:
   - Display shows elapsed time (MM:SS)
   - Press S1 to reset clock to 00:00
   - Press and hold S3 to show current voltage (X.XXV)

3. **Background Processes**:
   - Timer interrupt updates time every second
   - ADC continuously samples potentiometer
   - Min/max voltage values are tracked


