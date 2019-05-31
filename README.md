Arduino Core Support for Attiny 1 Series MCU
==============================================================================
# Links
  - [Documentation]((https:/tinycore.dev)
  - [Tiny Core 16 Board](https://www.tindie.com/products/xkimi/tiny-core-16-dev-board/)
  - [Programmer Board](https://www.tindie.com/products/xkimi/tiny-core-programmer/)
  
# Feature
 Specifications |  .
------------ | -------------
Flash (program memory)   | 32/16 KB
RAM  | 2 KB
EEPROM | 256 bytes
Bootloader | No
GPIO Pins | 18
ADC Channels | 10
PWM Channels | 3
Peripheral | USART, SPI, I2C, Touch
Clock | 20 MHz
Power Consumption | min 2.9μA, max 10mA

# Arduino Support
  Currently UART, I2C, SPI, basic timer functions like delay, delayMicroseconds, milis, micros are working, I'm working on adding EEPROM support.
 
# Programmer
 Attiny 1 Series use UDPI protocol for programming which only use 1 pin for programming which is PA0. 
 I made a ATMega32u4 firmware and a programmer board [link] for Attiny 1 Series.
 ATMega328p will also works.
  
# Installation
- Install the current upstream Arduino IDE at the 1.8.7 level or later. The current version is at the [Arduino website](http://www.arduino.cc/en/main/software).
- Start Arduino and open Preferences window.
- Enter ```https://raw.githubusercontent.com/xukangmin/TinyCore/master/package/package_tinycore_index.json``` into *Additional Board Manager URLs* field. You can add multiple URLs, separating them with commas.
- Open Boards Manager from Tools > Board menu and install *TinyCore* platform (and don't forget to select your TinyCore board from Tools > Board menu after installation).

# Pin Mapping
![Pin Mapping](/docs/tinycore16_pinmap.png)


# To-Do
