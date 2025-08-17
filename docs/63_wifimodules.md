---
title: WiFi Modules (ESP8266)
layout: home
parent: Microcontrollers & Communication Modules
nav_order: 63
---

# Wi-Fi Modules

## 1. Definition
**Wi-Fi Modules** allow microcontrollers to connect to wireless networks for internet-based communication.  
They are commonly used in **IoT (Internet of Things)** projects to send or receive data from web servers, cloud platforms, or mobile apps.  

Examples: **ESP8266, ESP32, NodeMCU, and ESP-01**.
<img src="\images\esp8266.jpg" width="500" height="300" alt="Wi-Fi module  example">



## 2. Features
- Provides **wireless connectivity** to devices.
- Supports **TCP/IP protocols** for internet communication.
- Can act as a **Wi-Fi client** (connect to a router) or **Wi-Fi Access Point (AP)**.
- Available as **standalone microcontrollers (ESP32, ESP8266)** or as **modules controlled via AT commands**.
- Supports **IoT platforms** like Blynk, Firebase, MQTT, and Google Cloud.



## 3. Applications
- **Home automation** (smart lights, fans, appliances).
- **IoT monitoring systems** (temperature, air quality, security).
- **Data logging** to the cloud or local server.
- **Remote control** using mobile apps or web dashboards.
- **Robotics** with wireless control.


## 4. How It Works
- The microcontroller communicates with the Wi-Fi module via **UART (TX/RX pins)** or runs directly on the module (e.g., ESP8266, ESP32).
- The module connects to a **Wi-Fi router** or creates its own hotspot.
- Data is sent/received through **HTTP, MQTT, or WebSocket protocols**.


## 5. Circuit Example
<img src="\images\Circuit-Diagram-of-ESP8266-Module.jpg" width="500" height="300" alt="Wi-Fi module circuit example">

- Connect **VCC → 3.3V** (some boards have regulators for 5V input).  
- **GND → Ground**.  
- **TX ↔ RX** with microcontroller (cross-connected).  
- **EN/CH_PD pin → HIGH (3.3V)** to enable the module.  



## 6. Code Example (ESP8266 with Arduino IDE)
```cpp
#include <ESP8266WiFi.h>

const char* ssid = "YourWiFi";
const char* password = "YourPassword";

void setup() {
  Serial.begin(115200);
  WiFi.begin(ssid, password);
  while (WiFi.status() != WL_CONNECTED) {
    delay(500);
    Serial.print(".");
  }
  Serial.println("Connected to WiFi!");
}

void loop() {
  // Add IoT code here
}
```


## 7. Video Explanation 
video coming soon