---
layout: page
title: Display and UI
nav_order: 4
permalink: /Transmitter/DisplayAndUI/
---

# Display and UI

The UI of the OpenScaleRemote Transmitter is build with [SquareLine Studio](https://squareline.io/) running on a [2,8 inch ILI9488](https://www.az-delivery.de/en/products/2-8-zoll-lcd-tft-touch-display) based tft witch capacitive touch. It uses the [TFT_eSPI](https://github.com/Bodmer/TFT_eSPI) display library by Bodmer and the [lvgl](https://lvgl.io/) grafics library by kisvegabor. Make sure that the tft matches the logic voltage of your mcu or use a SPI capable logic level voltage converter.
Due too the lack of SRAM on the Arduino MEGA 2560, the SquareLine Studio based UI is not available for this mcu.

ILI9488 TFT + Touch | Arduino MEGA 2560 | ESP32WROOM32 | Teensy4.1
-------- | -------- | -------- | --------
lcd_mosi | 51 | 23 | not defined
lcd_miso | 50 | 19 | not defined
lcd_sck | 52 | 18 | not defined
lcd_cs | 48 | 17 | not defined
lcd_reset | 49 | 16 | not defined
lcd_dc | 46 | 12 | not defined
touch_mosi | 51 | 23 | not defined
touch_miso | 50 | 19 | not defined
touch_sck | 52 | 18 | not defined
touch_cs | 47 | 4 | not defined