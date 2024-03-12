---
layout: page
title: Display and UI
nav_order: 4
permalink: /Transmitter/DisplayAndUI/
---

# Display and UI

There are different options for the UI for your OpenScaleRemote. The most powerfull is build with [SquareLine Studio](https://squareline.io/) running on a [2,8 inch ILI9488](https://www.az-delivery.de/en/products/2-8-zoll-lcd-tft-touch-display) based tft witch capacitive touch. It uses the [TFT_eSPI](https://github.com/Bodmer/TFT_eSPI) display library by Bodmer and the [lvgl](https://lvgl.io/) grafics library by kisvegabor. Make sure that the tft matches the logic voltage of your mcu or use a SPI capable logic level voltage converter.
Due too the lack of SRAM on the Arduino MEGA 2560, the SquareLine Studio based UI is not available for this mcu.  
The second option is a 2004 I2C LCD with a Rotary Encoder. This option is available for all supported mcus.

ILI9488 TFT + Touch | Arduino MEGA 2560 | ESP32WROOM32 | Teensy4.1
-------- | -------- | -------- | --------
lcd_mosi | not available (51) | 23 | not defined
lcd_miso | not available (50) | 19 | not defined
lcd_sck | not available (52) | 18 | not defined
lcd_cs | not available (48) | 17 | not defined
lcd_reset | not available (49) | 16 | not defined
lcd_dc | not available (46) | 12 | not defined
touch_mosi | not available (51) | 23 | not defined
touch_miso | not available (50) | 19 | not defined
touch_sck | not available (52) | 18 | not defined
touch_cs | not available (47) | 4 | not defined