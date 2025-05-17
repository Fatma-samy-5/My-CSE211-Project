<<<<<<< HEAD
![](./resources/official_armmbed_example_badge.png)
# Blinky Mbed OS example

The example project is part of the [Arm Mbed OS Official Examples](https://os.mbed.com/code/) and is the [getting started example for Mbed OS](https://os.mbed.com/docs/mbed-os/v5.14/quick-start/index.html). It contains an application that repeatedly blinks an LED on supported [Mbed boards](https://os.mbed.com/platforms/).

You can build the project with all supported [Mbed OS build tools](https://os.mbed.com/docs/mbed-os/latest/tools/index.html). However, this example project specifically refers to the command-line interface tool [Arm Mbed CLI](https://github.com/ARMmbed/mbed-cli#installing-mbed-cli).
(Note: To see a rendered example you can import into the Arm Online Compiler, please see our [import quick start](https://os.mbed.com/docs/mbed-os/latest/quick-start/online-with-the-online-compiler.html#importing-the-code).)

1. [Install Mbed CLI](https://os.mbed.com/docs/mbed-os/latest/quick-start/offline-with-mbed-cli.html).

1. Clone this repository on your system, and change the current directory to where the project was cloned:

    ```bash
    $ git clone git@github.com:armmbed/mbed-os-example-blinky && cd mbed-os-example-blinky
    ```

    Alternatively, you can download the example project with Arm Mbed CLI using the `import` subcommand:

    ```bash
    $ mbed import mbed-os-example-blinky && cd mbed-os-example-blinky
    ```


## Application functionality

The `main()` function is the single thread in the application. It toggles the state of a digital output connected to an LED on the board.

## Building and running

1. Connect a USB cable between the USB port on the board and the host computer.
2. <a name="build_cmd"></a> Run the following command to build the example project and program the microcontroller flash memory:
    ```bash
    $ mbed compile -m <TARGET> -t <TOOLCHAIN> --flash
    ```
The binary is located at `./BUILD/<TARGET>/<TOOLCHAIN>/mbed-os-example-blinky.bin`.

Alternatively, you can manually copy the binary to the board, which you mount on the host computer over USB.

Depending on the target, you can build the example project with the `GCC_ARM`, `ARM` or `IAR` toolchain. After installing Arm Mbed CLI, run the command below to determine which toolchain supports your target:

```bash
$ mbed compile -S
```

## Expected output
The LED on your target turns on and off every 500 milliseconds.


## Troubleshooting
If you have problems, you can review the [documentation](https://os.mbed.com/docs/latest/tutorials/debugging.html) for suggestions on what could be wrong and how to fix it.

## Related Links

* [Mbed OS Stats API](https://os.mbed.com/docs/latest/apis/mbed-statistics.html).
* [Mbed OS Configuration](https://os.mbed.com/docs/latest/reference/configuration.html).
* [Mbed OS Serial Communication](https://os.mbed.com/docs/latest/tutorials/serial-communication.html).
* [Mbed OS bare metal](https://os.mbed.com/docs/mbed-os/latest/reference/mbed-os-bare-metal.html).
* [Mbed boards](https://os.mbed.com/platforms/).

### License and contributions

The software is provided under Apache-2.0 license. Contributions to this project are accepted under the same license. Please see contributing.md for more info.

This project contains code from other projects. The original license text is included in those source files. They must comply with our license guide.
=======
# My-CSE211-Project
<<<<<<< HEAD
# Real-Time Clock and Analog Signal Display with Nucleo Board
#Link of the video🥰🥰:
Click here>>
[Project Demonstration](https://drive.google.com/file/d/1a5-6-lx1gGz0rocJ5X8RKrLVmOLAT9_K/view?usp=drivesdk)

Photos:[Click here](https://github.com/user-attachments/assets/b08f5873-c797-41bc-8e5b-3e91e0bd2bc5)
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


>>>>>>> 287ed3d83cbf48240b515b92e94d321a17764620
=======
>>>>>>> 101610178de6fe14cccca14bc4b44117896945cd
