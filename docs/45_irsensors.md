---
title: IR Sensors & Remotes
layout: home
parent: Input Devices & Sensors
nav_order: 45
---


# IR Sensors & Remotes

## 1. Definition
**IR (Infrared) Sensors** detect infrared light, which is invisible to our eyes but can be used for communication or object detection.  
They are commonly paired with **IR Remotes** to send commands wirelessly, similar to how your TV remote works.  

IR sensors can also detect objects or measure short distances by detecting reflected IR light.

<img src="\images\IR-.webp" width="500" height="300" alt="IR sensor module">

**IR Remote and Receiver Module**

<img src="\images\51ZOAZKpNcL.jpg" width="500" height="300" alt="IR remote and receiver">

## 2. Features

- **Wireless Communication:** Send and receive commands without wires.
- **Short Range:** Typically works within 1–5 meters for remotes, a few centimeters for object detection.
- **Low Cost:** Affordable for most projects.
- **Multiple Uses:** Remote control, object detection, line-following robots, and automation.
- **Easy to Interface:** Works with Arduino, Raspberry Pi, and other microcontrollers.

## 4. How to Use

### 4.1. Identify the Pins
- **For IR Receiver Module (e.g., VS1838B):**
  - **OUT:** Signal output pin.
  - **GND:** Ground connection.
  - **VCC:** 3.3V or 5V power input.
- **For IR Emitter LED:** Just like a normal LED, but emits IR light.
- **For IR Obstacle Sensor Module:**
  - VCC → Power input.
  - GND → Ground.
  - OUT → Digital output (HIGH/LOW).

### 4.2. Choose the Right Module
- **Remote + Receiver Kit:** For controlling devices with an IR remote.
- **IR Obstacle Sensor:** For detecting objects in front of the sensor.
- **Line Sensor Array:** For detecting black/white lines in robotics.

### 4.3. Connect It Correctly
- **IR Receiver to Arduino:**
  - VCC → 5V
  - GND → GND
  - OUT → Any digital pin (e.g., D2)
- **Obstacle Sensor to Arduino:**
  - Same wiring, but OUT pin will go HIGH or LOW depending on object detection.
- Keep the receiver facing the remote for reliable signal.

### 4.4. Test It
- For remotes:
  - Use the Arduino **IRremote** library to read button codes in the Serial Monitor.
  - Save these codes to trigger actions (e.g., turn on an LED).
- For object sensors:
  - Place an object in front and see if the module’s onboard LED lights up.
  - Read the output pin in Arduino to see detection status.

### 4.5. Mount Securely
- ***On breadboard:*** Use jumper wires.
- ***On robots/projects:*** Fix in place so the sensor faces the correct direction.
- Avoid bright sunlight, it can interfere with IR signals.

 **Tip:** IR remotes work best indoors, as sunlight contains infrared light that can cause interference.

## 5. Video Explanation

video coming soon