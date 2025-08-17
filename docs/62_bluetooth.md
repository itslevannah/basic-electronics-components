---
title: Bluetooth Modules (HC-05/06)
layout: home
parent: Microcontrollers & Communication Modules
nav_order: 62
---


# Bluetooth Modules

## 1. Definition
**Bluetooth Modules** enable short-range **wireless communication** between microcontrollers (like Arduino, ESP32) and other devices such as smartphones, laptops, or PCs.  
They are commonly used for **wireless control, data exchange, and IoT projects**.  

Popular modules include **HC-05** and **HC-06**.

<img src="\images\Bluetooth-Module-HC05.webp" width="500" height="300" alt="Bluetooth module examples">



## 2. Types of Bluetooth Modules
- **HC-05** → Can act as **Master or Slave** (two-way communication).
- **HC-06** → Works only as **Slave** (simple pairing with Master device).
- **BLE Modules (like HM-10, ESP32 built-in)** → Support **Bluetooth Low Energy**, better for low-power IoT.



## 3. Pin Configuration (HC-05 / HC-06)
- **VCC** → Power supply (3.6V–6V, typically 5V).  
- **GND** → Ground.  
- **TXD** → Transmit data (to Arduino RX).  
- **RXD** → Receive data (from Arduino TX, use voltage divider if 5V).  
- **EN/KEY (optional)** → Used for AT Command mode (configuration).



## 4. How It Works
1. Connect the module to Arduino (TX ↔ RX).  
2. Pair it with a **Bluetooth-enabled device** (phone/laptop).  
3. Use a **serial communication app** to send/receive data.  
4. Arduino processes the received data and performs actions (e.g., turn on LED, control motor).  


## 5. Applications
- Wireless robot control.  
- Home automation (lights, fans, appliances).  
- Wireless sensor data logging.  
- Remote-controlled cars/drones.  
- IoT devices (basic Bluetooth communication).  


## 6. Safety & Notes
- Use a **voltage divider** for RX pin if connecting to a 5V Arduino.  
- Keep distance within **10 meters** (classic modules).  
- Do not expose to **electrical shorts or water**.  
- Default HC-05 settings → `9600 baud`, PIN: `1234` or `0000`.  


## 7. Video Explanation 
video coming soon