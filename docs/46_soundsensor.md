---
title: Sound Sensors (Microphones)
layout: home
parent: Input Devices & Sensors
nav_order: 46
---



# Sound Sensors

## 1. Definition
**Sound Sensors** detect sound levels in the environment and convert them into electrical signals.  
They are commonly used in projects where you want the device to **react to claps, voice commands, or other noises**.

Sound sensors can be **analog** (provide varying voltage based on sound intensity) or **digital** (trigger HIGH/LOW output when sound crosses a certain threshold).

<img src="\images\71nl2sZhO2L.jpg" width="500" height="300" alt="Sound sensor module">

**Typical Sound Sensor Module**

<img src="\images\Arduino-Sound-Detection-Sensor-Pin-Outs.png" width="500" height="300" alt="Sound sensor module pins">

## 2. Features

- **Sound Detection:** Detects claps, voices, or ambient noise.
- **Digital & Analog Output:** Choose depending on project needs.
- **Adjustable Sensitivity:** Many modules have a potentiometer to set the detection threshold.
- **Low Cost & Easy to Use:** Ideal for beginners.
- **Compatible:** Works with Arduino, Raspberry Pi, and other microcontrollers.
- **Versatile Applications:** Clap switches, sound-activated lights, noise monitoring, interactive robots.

## 4. How to Use

### 4.1. Identify the Pins
- **VCC:** Power input (3.3V–5V).  
- **GND:** Ground connection.  
- **DO (Digital Output):** Goes HIGH when sound exceeds threshold.  
- **AO (Analog Output):** Provides voltage proportional to sound intensity.

### 4.2. Adjust Sensitivity
- Turn the onboard **potentiometer** to set how loud a sound must be to trigger the digital output.  
- Start low and increase until the sensor reliably detects your target sound.

### 4.3. Connect It Correctly
- **Digital Output to Arduino:**
  - VCC → 5V  
  - GND → GND  
  - DO → Any digital pin (e.g., D2)  
- **Analog Output to Arduino:**
  - VCC → 5V  
  - GND → GND  
  - AO → Any analog pin (e.g., A0)  

### 4.4. Test It
- **Digital Output:** Clap or make noise; the digital pin should read HIGH.  
- **Analog Output:** Use Arduino **Serial Monitor** to see voltage changes based on sound intensity.  
- Trigger LEDs, buzzers, or motors based on detected sound.

### 4.5. Mount Securely
- Place the sensor where it can clearly "hear" sounds.  
- Avoid placing near constant noise sources if not needed.  
- Use jumper wires or screws to fix the sensor module in your project.

 **Tip:** Digital sound sensors are great for simple clap switches, while analog outputs give more flexibility for sound-level monitoring.

## 5. Video Explanation

video coming soon