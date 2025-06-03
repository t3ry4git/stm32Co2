# stm32Co2

A simple CO2 and environmental monitor based on the STM32F103C8 microcontroller. The firmware reads temperature and humidity from a DHT22 sensor, measures CO2 concentration using an MHZ19B module and displays values on an SSD1306 OLED screen.

## Hardware requirements

- **MCU:** STM32F103C8 ("Blue Pill" or compatible)
- **Temperature/Humidity sensor:** DHT22
- **CO2 sensor:** MHZ19B (UART interface)
- **Display:** SSD1306 I2C OLED

## Building with STM32CubeIDE

1. Open the `test.ioc` project file in STM32CubeIDE.
2. Let CubeIDE generate the project files if prompted.
3. Build the `test` target from the IDE. Default settings produce both `Debug` and `Release` outputs.
4. Flash the resulting binary to your board using the built‑in CubeIDE programmer or an external tool such as ST‑Link.

## Third‑party software

This repository includes STM32 HAL drivers from STMicroelectronics under the BSD‑3‑Clause license as found in `Drivers/STM32F1xx_HAL_Driver/LICENSE.txt`. The SSD1306 display driver and font code in `Core/Src` and `Core/Inc` are distributed under the GNU GPL version 3.

