---
title: Hall Effect Sensors
layout: home
parent: Input Devices & Sensors
nav_order: 48
---



# Hall Effect Sensors

## 1. Definition
A **Hall Effect Sensor** detects magnetic fields and converts them into an electrical signal.  
It works on the **Hall Effect** principle, where a voltage is generated when a magnetic field passes through a conductor or semiconductor.  

These sensors are used for speed detection (in fans, wheels), position sensing, proximity sensing, and even in brushless DC motors.

<img src="\images\images\F2166231-01.webp" width="500" height="300" alt="hall effect sensor module">

**Hall Effect Sensor Symbol**

<img src="\images\Hall_effect_sensor_circuit_symbol.svg.png" width="500" height="300" alt="hall effect symbol">

## 2. Features

- **Magnetic Field Detection:** Can sense the presence, strength, or direction of a magnetic field.
- **Contactless Sensing:** No physical contact needed, reduces wear and tear.
- **High Reliability:** Works in dusty, dirty, or wet environments where mechanical switches might fail.
- **Types:**
  - **Analog:** Output changes smoothly with magnetic field strength.
  - **Digital:** Output is either ON or OFF depending on magnetic field detection.
- **Non-Polarized Sensing Face:** Detects magnets from either pole (some sensors are pole-specific).

## 4. How to Use

### 4.1. Identify the Pins (e.g., A3144 Hall Sensor)
- **VCC:** Connect to 5V or 3.3V (check datasheet).
- **GND:** Ground connection.
- **OUT:** Signal output pin.

<img src="\images\20180901093736_98867.jpg" width="500" height="300" alt="hall effect sensor pins">

### 4.2. Choose the Right Type
- **Digital Hall Sensor:** For detecting if a magnet is present or not (e.g., A3144).
- **Analog Hall Sensor:** For measuring magnetic field strength (e.g., SS49E).
- **Latching Hall Sensor:** Turns ON with one pole, OFF with the opposite pole, good for rotation tracking.

### 4.3. Connect It Correctly
- **To Arduino:**
  - VCC → 5V  
  - GND → GND  
  - OUT → Any digital pin (digital sensor) or analog pin (analog sensor)
- Place the sensor so the flat face points toward the magnet.
- Keep wiring short for cleaner signals.

### 4.4. Test It
- For **digital sensors**:
  - Bring a magnet close → output goes LOW (or HIGH depending on type).
  - Remove the magnet → output returns to normal.
- For **analog sensors**:
  - Read the voltage from the OUT pin.
  - Voltage changes as magnet moves closer or farther.
- Use Arduino’s Serial Monitor to see the readings in real time.

### 4.5. Mount Securely
- ***On breadboard:*** Use jumper wires for quick testing.
- ***In projects:*** Fix with glue, screws, or brackets so it stays aligned with the magnet.
- Avoid placing it near strong stray magnetic fields unless they are part of your measurement.

 **Tip:** Hall sensors won’t detect non-magnetic materials like plastic, wood, or aluminum, they only react to magnets.

## 5. Video Explanation

video coming soon