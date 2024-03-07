---
layout: page
title: Model Data Storage
nav_order: 5
permalink: /Transmitter/ModelDataStorage/
---

# Model data storage

The OpenScaleRemote Transmitter uses a SD-Card to store model spezific data such as name, servo directions and servo limits. Any SD or MicroSD card module can be used here.

SD-Card | Arduino MEGA 2560 | ESP32WROOM32 | Teensy4.1
-------- | -------- | -------- | --------
sd_mosi | 51 | 23 | not defined
sd_miso | 50 | 19 | not defined
sd_sck | 52 | 18 | not defined
sc_cs | 44 | 13 | not defined