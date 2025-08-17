---
title: Power Supply Modules
layout: home
parent: Power Sources & Protection
nav_order: 40
---



# Power Supply Modules

## 1. Definition
A **Power Supply Module** is a small circuit board or device that takes power from a source (like a wall plug, battery, or USB) and changes it into the voltage your project or device needs.  
They save you from building a full power circuit from scratch and are used in things like phone chargers, Arduino projects, LED strips, and small robots.

<img src="\images\61N9VWw2GqL.jpg" width="500" height="300" alt="power supply module">

**Common Power Supply Module Symbols**

<img src="\images\imagessupply.png" width="500" height="300" alt="power supply symbol"> 

## 2. Features

- **Changes Voltage:** Can lower (step-down) or raise (step-up) voltage, and can also convert AC to DC.
- **Steady Output:** Keeps voltage stable even if your device’s power use changes.
- **Multiple Outputs:** Some give more than one voltage at the same time (e.g., 3.3V and 5V).
- **Plug-and-Play:** Works straight away without needing extra building.
- **Built-in Protection:** Often has short-circuit, overvoltage, and overheating protection.

## 4. How to Use

### 4.1. Identify Input and Output
- **Input:** Where you connect your power source (could be a wall adapter, battery, or USB).
- **Output:** Where you connect the device or circuit you want to power.
- **GND:** The ground/common wire for both input and output.

<img src="\images\MB102-Breadboard-Power-Supply-Module-Overview.jpg" width="500" height="300" alt="power supply module pins">

 **Safety Tip:** If the input is AC mains (like 220V from a wall socket), **be extremely careful** ,this can cause electric shock.

### 4.2. Choose the Right Module
- **Input Voltage Range:** Must match your power source (e.g., a 12V battery).
- **Output Voltage & Current:** Must match your device’s needs (e.g., 5V for Arduino).
- **Type:** Linear (simpler, less efficient) or switching (more efficient, cooler).
- **Size and Shape:** Make sure it fits in your project space.

### 4.3. Connect It Correctly
- **Check Polarity:** Always connect positive (+) to positive, and negative (–) to negative.
- Use thicker wires for higher current devices like motors.
- For AC input modules, keep all connections insulated.

### 4.4. Test Before Use
- Use a **multimeter** to check the output voltage before connecting sensitive electronics.
- If the module is adjustable, turn the small screw (potentiometer) to set your desired voltage.
- Check for heating if powering something that draws a lot of current.

### 4.5. Mount Securely
- ***On breadboard:*** Use pin headers if the module supports them.
- ***On PCB:*** Solder it firmly in place.
- ***Standalone:*** Place it inside a protective case to avoid touching live parts.

## 5. Video Explanation

video coming soon