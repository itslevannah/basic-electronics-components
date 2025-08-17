---
title: ESP8266 / ESP32
layout: home
parent: Microcontrollers & Communication Modules
nav_order: 60
---



# ESP8266 / ESP32

## 1. Definition
**ESP8266** and **ESP32** are Wi-Fi-enabled microcontrollers commonly used in **IoT (Internet of Things)** projects.  
- The **ESP8266** is low-cost and good for simple Wi-Fi projects.  
- The **ESP32** is more powerful, with built-in **Wi-Fi + Bluetooth**, dual-core processing, more GPIOs, and support for advanced projects.  

They are great for connecting devices to the internet and building **smart systems**.

<img src="\images\6e9dbaf653fd34ddb00442bea067a635.png" width="500" height="300" alt="ESP8266 and ESP32 boards">



## 2. Key Features

### 3.1 ESP8266
- **Wi-Fi support** (2.4 GHz)  
- Lower cost and lower power  
- Limited GPIO pins (~11 usable)  
- Single-core processor  

### 3.2. ESP32
- **Wi-Fi + Bluetooth (Classic + BLE)**  
- Dual-core processor (faster & more powerful)  
- More GPIOs (~30 usable)  
- Built-in **ADC, DAC, capacitive touch, PWM, SPI, I2C, UART**  
- Supports **deep sleep** (low power IoT devices)


### 3.3. ESP8266 vs ESP32 Comparison


| Feature              | ESP8266                          | ESP32                                    |
|----------------------|----------------------------------|------------------------------------------|
| **Release Year**     | 2014                             | 2016                                     |
| **Processor**        | Single-core Tensilica L106 (80–160 MHz) | Dual-core Tensilica Xtensa LX6 (160–240 MHz) |
| **RAM**              | ~160 KB                         | ~520 KB (with external PSRAM options)     |
| **Flash Memory**     | Typically 4 MB                  | 4–16 MB (varies by module)               |
| **Wi-Fi**            | 2.4 GHz only                    | 2.4 GHz + better speed & stability       |
| **Bluetooth**        |  Not supported                  |  Bluetooth 4.2 & BLE support            |
| **GPIO Pins**        | ~17 usable pins                 | 30+ pins (depending on board)            |
| **Analog Inputs**    | 1 (10-bit ADC)                  | Up to 18 (12-bit ADC)                    |
| **PWM Support**      |  Yes                            |  Yes (more channels & higher resolution)|
| **Communication**    | UART, SPI, I²C                  | UART, SPI, I²C, CAN, I²S                 |
| **Power Consumption**| Low                             | Ultra-low power modes available          |
| **Cost**             | Cheaper (~$2–4)                 | Slightly more expensive (~$5–8)          |
| **Best For**         | Simple IoT projects, Wi-Fi apps | Advanced IoT, Bluetooth + Wi-Fi projects |

## Summary
- Use **ESP8266** if you want a **cheap, simple Wi-Fi board** for small IoT projects.  
- Use **ESP32** if you need **more power, more pins, Bluetooth, or multiple sensors**.  


## 3. Applications
- Smart home automation (lights, fans, appliances)  
- IoT projects (weather station, soil monitoring, etc.)  
- Remote sensors with Wi-Fi or Bluetooth data transfer  
- Robotics (Wi-Fi controlled robots)  
- Wearables and portable devices  


## 4. Pinout Examples

### ESP8266 (NodeMCU)
- **D0–D8** → Digital pins  
- **A0** → Analog input  
- **3.3V / GND** → Power supply  
- **TX/RX** → Serial communication  

### ESP32 (DevKit)
- **GPIOs** → Multiple digital pins  
- **ADC/DAC** → For analog input/output  
- **TX0/RX0, TX1/RX1** → UART communication  
- **EN** → Reset pin  
- **3.3V / GND** → Power supply  



## 5. Example Code

### Blink an LED (ESP8266/ESP32)

```cpp
int led = 2; // On-board LED (D4 on ESP8266, GPIO2 on ESP32)

void setup() {
  pinMode(led, OUTPUT);
}

void loop() {
  digitalWrite(led, HIGH); // LED ON
  delay(1000);
  digitalWrite(led, LOW);  // LED OFF
  delay(1000);
}
```

## 6. Video Explanation
Video coming soon