# stm32_f407_ili9488_lvgl_demo


A demo for Zephyr RTOS to shows how to using LVGL with a 3.5" TFT LCD.


## Requirements

Set the environment variable `GCC_ARM_HOME` to the directory of your GCC embedded tool-chain or you can change `CMakeLists.txt` directly.

* A STM32F407VET6 development board ("black_f407ve").
* A TFT LCD with ILI9488 IC SPI driver - 480x320.

## Getting Started

```cmd
west build -b black_f407ve
west flash
```


![Image1](docs/demo1.jpg)