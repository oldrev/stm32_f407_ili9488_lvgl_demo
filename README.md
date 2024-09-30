# STM32F407 ILI9488 LVGL Demo

***Warning: Out dated!***

This demo showcases how to integrate LVGL (Light and Versatile Graphics Library) with a 3.5" TFT LCD using Zephyr RTOS on an STM32F407VET6 development board.

## Requirements

Before you begin, ensure you have the following:

- **Zephyr RTOS**: Version 2.5.0
- **STM32F407VET6 Development Board**: Also known as "black_f407ve".
- **TFT LCD**: A 3.5" TFT LCD with an ILI9488 IC and SPI driver, supporting a resolution of 480x320.

### Toolchain Setup

Set the environment variable `GCC_ARM_HOME` to the directory of your GCC embedded toolchain. Alternatively, you can modify the `CMakeLists.txt` file directly.

## Getting Started

To build and flash the demo onto your STM32F407VET6 board, follow these steps:

```cmd
west build -b black_f407ve
west flash
```


![Image1](docs/demo1.jpg)
