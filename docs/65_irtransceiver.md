---
title: IR Transmitter/Receiver
layout: home
parent: Microcontrollers & Communication Modules
nav_order: 65
---



# IR Transmitter & Receiver

## 1. Definition
**IR (Infrared) Transmitter and Receiver Modules** are used for wireless communication using infrared light, invisible to the human eye.  
They are widely used in remote controls, obstacle detection, and short-range data transfer.

<img src="\images\51awSdpmDtL._UF1000,1000_QL80_.jpg" width="500" height="300" alt="IR Transmitter and Receiver modules">



## 2. Components
- **IR Transmitter (LED):** Emits infrared light.  
- **IR Receiver (Photodiode/Phototransistor):** Detects the incoming IR signals.  
- **Driver Circuit:** Optional, used for modulation and demodulation of signals.  



## 3. Features
- Short-range wireless communication (a few centimeters to a few meters).  
- Low cost and easy to use.  
- Requires **line of sight** between transmitter and receiver.  
- Immune to radio frequency interference.  



## 4. Applications
- **Remote controls** (TV, AC, audio systems).  
- **Obstacle detection** in robots.  
- **Data transfer** in simple electronics projects.  
- **Object counters** and automation systems.  


## 5. Example Code (Arduino)

```cpp
// IR Receiver example
#include <IRremote.h>

int RECV_PIN = 11;      // Pin connected to IR receiver
IRrecv irrecv(RECV_PIN);
decode_results results;

void setup() {
  Serial.begin(9600);
  irrecv.enableIRIn(); // Start the receiver
}

void loop() {
  if (irrecv.decode(&results)) {
    Serial.println(results.value, HEX); // Print IR code in HEX
    irrecv.resume(); // Receive the next value
  }
}
```
## 6. Video Explanation 
video coming soon