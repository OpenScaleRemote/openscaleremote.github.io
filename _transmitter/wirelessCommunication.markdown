---
layout: page
title: Wireless Communication
nav_order: 2
permalink: /Transmitter/WirelessCommunication/
---

# Wireless communication

The OpenScaleRemote uses an [RFM95W LoRa module](https://www.hoperf.com/modules/lora/RFM95W.html) build by HopeRF running the [LoRa](https://github.com/sandeepmistry/arduino-LoRa) library by Sandeep Mistry. You can choose between different types of RFM95W boards. We recommend the [adafruit version](https://www.adafruit.com/product/3072), but any other board can be used too. Just make sure that it matches the logic voltage of your mcu or use a SPI capable logic level voltage converter.

RFM95W | Arduino MEGA 2560 | ESP32WROOM32 | Teensy4.1
-------- | -------- | -------- | --------
rfm95w_mosi | 51 | 23 | not defined
rfm95w_miso | 50 | 19 | not defined
rfm95w_sck | 52 | 18 | not defined
rfm95w_cs | 53 | 5 | not defined
rfm95w_reset | 10 | 14 | not defined
rfm95w_dio0 | 2 | 2 | not defined