---
title: LDR / Photoresistors
layout: home
parent: Input Devices & Sensors
nav_order: 42
---



# LDR / Photoresistors

## 1. Definition
An **LDR** (Light Dependent Resistor) or **Photoresistor** is a special type of resistor that changes its resistance based on the amount of light falling on it.  
- In bright light, its resistance goes down.  
- In darkness, its resistance goes up.  

They are often used in night-lights, solar garden lamps, light meters, and streetlights that turn on automatically at night.

<img src="\images\31KqzDKiIbL._UF1000,1000_QL80_.jpg" width="500" height="300" alt="ldr photoresistor">

**LDR Symbol**

<img src="\images\small.png" width="500" height="300" alt="ldr symbol">

## 2. Features

- **Light Sensitive:** Resistance changes depending on light intensity.
- **Non-Polarized:** Can be connected in any direction.
- **Slow Response:** Works for detecting gradual changes in light, not fast flashes.
- **Low Cost & Simple:** Easy to use in beginner projects.

## 4. How to Use

### 4.1. Identify the LDR
- Looks like a small round or square disc with zig-zag lines on top.
- Two metal legs for connecting into a circuit.

<img src="\images\20250520121504406.png" width="500" height="300" alt="ldr identify">

### 4.2. Choose the Right LDR
- **Light Range:** Some LDRs are more sensitive to dim light, others to bright light.
- **Size:** Larger ones generally have a bigger light-sensitive area.
- **Resistance Range:** Common LDRs range from a few hundred ohms in bright light to several megaohms in darkness.

### 4.3. Connect It Correctly
- LDRs are **non-polarized**, so you can connect either leg to positive or negative.
- Usually used in a **voltage divider** with another resistor to turn light levels into measurable voltage for a microcontroller (like Arduino).
- Keep the light-sensitive face uncovered and pointed towards the light you want to measure.

### 4.4. Test It
- Use a **multimeter** in resistance mode:
  - Shine a light on it → resistance drops.
  - Cover it with your hand → resistance rises.
- If using with Arduino or similar, read the analog value to see changes in light level.

### 4.5. Mount Securely
- ***On breadboard:*** Push the legs into the holes.
- ***On PCB:*** Solder the legs into the pads.
- Avoid bending the legs too close to the body to prevent damage.

## 5. Video Explanation

video coming soon