---
title: Ultrasonic Sensors (HC-SR04)
layout: home
parent: Input Devices & Sensors
nav_order: 44
---

# Ultrasonic Sensors (HC-SR04)

## 1. Definition
An **Ultrasonic Sensor** like the **HC-SR04** measures distance by sending out high-frequency sound waves (ultrasound) and timing how long they take to bounce back from an object.  
It’s like how bats “see” in the dark using sound!  

These sensors are commonly used in obstacle avoiding robots, parking assistance systems, liquid level detection, and security alarms.

<img src="\images\imagessesor.jpg" width="500" height="300" alt="hc-sr04 ultrasonic sensor">

**HC-SR04 Pin Diagram**

<img src="\images\Introduction-to-HC-SR04.jpg" width="500" height="300" alt="hc-sr04 pinout">

## 2. Features

- **Non-Contact Measurement:** Measures distance without touching the object.
- **Range:** Typically 2 cm to 400 cm (0.8" to 13 feet).
- **Accuracy:** Around ±3 mm.
- **Easy to Interface:** Works with Arduino, Raspberry Pi, and other microcontrollers.
- **Low Cost:** Popular choice for beginners in robotics.

## 4. How to Use

### 4.1. Identify the Pins
- **VCC:** Connect to 5V power.
- **GND:** Ground connection.
- **TRIG:** Trigger pin, sends out the ultrasonic pulse.
- **ECHO:** Echo pin, receives the signal and sends back the time taken.

### 4.2. Choose the Right Module
- Standard HC-SR04 works well for most beginner projects.
- For harsh environments, choose waterproof ultrasonic sensors.
- If working in tight spaces, consider smaller modules like the HC-SR04P.

### 4.3. Connect It Correctly
- **Wiring to Arduino Example:**
  - VCC → 5V  
  - GND → GND  
  - TRIG → Any digital pin (e.g., D9)  
  - ECHO → Any digital pin (e.g., D10)
- Keep the sensor’s “eyes” (transducers) facing the object you want to measure.
- Avoid placing it too close to the ground or walls, as sound may bounce incorrectly.

### 4.4. Test It
- Use an Arduino example sketch:
  - Send a short pulse to TRIG.
  - Measure time until ECHO pin goes HIGH.
  - Distance = (Time × Speed of Sound) ÷ 2.
- Open the Serial Monitor to see distance readings in cm or inches.

### 4.5. Mount Securely
- ***On breadboard:*** Use jumper wires to connect it.
- ***On robot chassis or project box:*** Use screws or brackets to keep it fixed and facing forward.

 **Tip:** Ultrasonic sensors may have trouble with soft or angled surfaces that don’t reflect sound well.

## 5. Video Explanation

video coming soon