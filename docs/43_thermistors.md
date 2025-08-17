---
title: Thermistors / Temperature Sensors
layout: home
parent: Input Devices & Sensors
nav_order: 43
---


# Thermistors / Temperature Sensors

## 1. Definition
A **Thermistor** is a special type of resistor whose resistance changes with temperature.  
- **NTC (Negative Temperature Coefficient):** Resistance decreases when temperature increases.  
- **PTC (Positive Temperature Coefficient):** Resistance increases when temperature increases.  

They are widely used in temperature sensing for fans, air conditioners, 3D printers, digital thermometers, and battery packs.

<img src="\images\imagesthermistor.jpg" width="500" height="300" alt="thermistor example">

**Thermistor Symbol**

<img src="\images\thermistor-2.png" width="500" height="300" alt="thermistor symbol">

## 2. Features

- **Temperature Sensitive:** Resistance changes with heat or cold.
- **Non-Polarized:** Can be connected in any direction.
- **High Accuracy:** Especially in narrow temperature ranges.
- **Low Cost:** Easy to use in DIY and commercial devices.

## 4. How to Use

### 4.1. Identify the Thermistor
- Small bead, disc, or cylinder shape with two legs.
- Often marked as **NTC** or **PTC**.
- Sometimes covered in epoxy or glass for protection.

<img src="\images\thermistoridentity.png" width="500" height="300" alt="thermistor identify">

### 4.2. Choose the Right Thermistor
- **Type:** NTC for most temperature sensing; PTC for overcurrent or overheating protection.
- **Temperature Range:** Match your application (e.g., –40°C to +125°C for general use).
- **Resistance Value at 25°C:** Common values are 10kΩ, 100kΩ.
- **Tolerance:** Accuracy of measurement (e.g., ±1%, ±5%).

### 4.3. Connect It Correctly
- Thermistors are **non-polarized**, so either leg can go to positive or negative.
- Usually used in a **voltage divider** with another resistor to create a voltage signal that changes with temperature.
- Keep the sensor in good thermal contact with what you want to measure.

### 4.4. Test It
- Use a **multimeter** in resistance mode:
  - Warm it gently with your fingers → resistance changes.
  - Cool it down (ice pack) → resistance changes in the opposite way.
- If using with Arduino or similar, connect to an analog input and read the voltage change.

### 4.5. Mount Securely
- ***On breadboard:*** Push the legs into the holes.
- ***On PCB:*** Solder the legs firmly.
- Keep away from direct sunlight or drafts unless that’s part of your measurement.

## 5. Video Explanation

video coming soon