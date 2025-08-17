---
title: DC-DC Buck Converters
layout: home
parent: Power Sources & Protection
nav_order: 39
---

# Buck Converter (DC-DC)

## 1. Definition
A **Buck Converter** is a type of DC-DC switching regulator that steps down a higher DC voltage to a lower DC voltage efficiently, using an inductor, a switch (transistor), a diode, and a capacitor.

<img src="\images\lm2596-dc-dc-buck-converter-step-down-power-module-robodo-original-imaf7pamysgtgc7u.webp" width="500" height="300" alt="buck converter">

**Buck Converter Circuit Symbol**

<img src="\images\CC-CC-converter.png" width="500" height="300" alt="buck converter symbol"> 

## 2. Features

- **Voltage Step-Down:** Converts a higher DC input voltage to a lower DC output voltage.
- **High Efficiency:** Typically 80–95%, much higher than linear regulators.
- **Load Handling:** Can supply higher output current compared to a similar-sized linear regulator.
- **Adjustable Output:** Some modules allow setting the output voltage via a potentiometer.
- **Switching Frequency:** Usually ranges from 100 kHz to several MHz.

## 4. How to Use

### 4.1. Identify Input and Output Terminals
- **VIN:** Connect to the higher DC voltage source (e.g., 12V from battery).
- **VOUT:** Connect to the load requiring lower DC voltage (e.g., 5V for microcontroller).
- **GND:** Common ground for input and output.

<img src="\images\Mini360-pinout.jpg" width="500" height="300" alt="buck converter pins">

### 4.2. Choose the Right Module
- Input voltage range (must be above desired output voltage).
- Maximum output current rating.
- Efficiency rating and thermal performance.
- Adjustable vs fixed output voltage.

### 4.3. Connect It Correctly
- **Polarity Matters:** Ensure VIN is connected with correct polarity to avoid damage.
- Use proper gauge wires for higher currents.
- Add input/output capacitors if required to reduce voltage ripple.

### 4.4. Test Output Voltage
- Use a **multimeter** to measure the output before connecting sensitive electronics.
- Adjust the output voltage (if adjustable) using the onboard potentiometer.
- Check for voltage ripple if powering noise-sensitive circuits.

### 4.5. Mount It Securely
- ***On breadboard:*** Some small modules have pin headers for breadboard use.
- ***On PCB:*** Solder the module or components in place with proper heat dissipation.

## 5. Video Explanation

video coming soon