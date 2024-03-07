---
layout: page
title: MCU
nav_order: 2
permalink: /Transmitter/mcu/
---

# MCU

The software of the OpenScaleRemote has support for the following boards already implemented. But you can also use any other Board with support for SPI, I2C, GPIO based interrupts and a sufficient number of analog and digital input pins.  
Due to the lack of GPIO based interrupts the RP2040 running the arduino core by earlphilflower is not supported.

Board function | Arduino MEGA 2560 | ESP32WROOM32 | Teensy4.1
-------- | -------- | -------- | --------
pin_led | LED_BUILTIN | 2 | not defined
bat_voltage | not defined | 15 | not defined