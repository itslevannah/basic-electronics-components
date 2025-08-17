---
title: AVR ATmega328
layout: home
parent: Microcontrollers & Communication Modules
nav_order: 61
---



# AVR ATmega328

## 1. Definition
The **ATmega328** is an **8-bit AVR microcontroller** from Microchip (formerly Atmel).  
It is widely used in **Arduino Uno** boards and other DIY electronics projects.  
Known for being beginner-friendly, it balances performance, ease of programming, and affordability.

<img src="\images\ATMEGA328P-PU.jpg" width="400" height="250" alt="ATmega328 microcontroller">


## 2. Features
- **Architecture:** 8-bit AVR RISC
- **Clock Speed:** Up to 20 MHz
- **Flash Memory:** 32 KB (with 0.5 KB reserved for bootloader)
- **SRAM:** 2 KB
- **EEPROM:** 1 KB
- **I/O Pins:** 23 general-purpose pins
- **Timers:** 3 (two 8-bit, one 16-bit)
- **ADC:** 10-bit, up to 6 channels
- **Communication:** UART, SPI, I²C (TWI)
- **Operating Voltage:** 1.8V – 5.5V
- **Packages:** Available in DIP-28, TQFP, QFN



## 3. Pinout (DIP-28 Package)
- **Digital I/O:** 14 pins (D0–D13, some with PWM support)
- **Analog Inputs:** 6 pins (A0–A5)
- **Power Pins:** VCC, AVCC, GND, AREF
- **Reset Pin:** External reset option



## 4. Common Uses
- Arduino Uno and Nano boards  
- Robotics and automation projects  
- IoT devices (when combined with WiFi modules like ESP8266/ESP32)  
- Sensor interfacing and control systems  
- Educational electronics kits  



## 5. Advantages
- Popular and well-documented  
- Supported by **Arduino IDE** and other toolchains  
- Large community and open-source libraries available  
- Low power consumption in sleep modes  
- Cheap and easy to source  


## 6. Limitations
- Limited memory compared to modern microcontrollers  
- Slower than 32-bit ARM/ESP chips  
- No built-in WiFi or Bluetooth  
- Limited ADC resolution (10-bit)  


## 7. Example Applications
- Blinking LED (Hello World of electronics)  
- Reading analog sensor values  
- Driving motors with PWM  
- Serial communication with PCs or other devices  
- DIY weather stations, clocks, and small robots  

## 8. Video Explanation
Video coming soon