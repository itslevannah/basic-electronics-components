---
title: Transistors 
layout: home
parent: Basic Active Components
nav_order: 24
---

# Transistors (NPN/PNP)

## 1. Definition
### 1.1 Transistor

A transistor is a semiconductor device used to amplify or switch electronic signals.  
It has three terminals that control the flow of current: **Base (B)**, **Collector (C)**, and **Emitter (E)**.


<img src="\images\Types-of-Transistors.jpg" width="500" height="300" alt="Transistor examples">

**Transistor Symbol**

<img src="\images\techart_symbols2_1.webp" width="500" height="300" alt="Transistor symbols">


### 1.2 NPN vs PNP Transistors

#### **NPN Transistor**
- **Symbol:** Arrow points **out** of the emitter.
- **Operation:** Current flows from **collector to emitter** when a small current enters the base.
- **Biasing:** Base is more positive than emitter.
- **Common Use:** Low-side switching (connect emitter to ground).

#### **PNP Transistor**
- **Symbol:** Arrow points **in** to the emitter.
- **Operation:** Current flows from **emitter to collector** when a small current leaves the base.
- **Biasing:** Base is more negative than emitter.
- **Common Use:** High-side switching (connect emitter to supply voltage).

**Side-by-side comparison:**

| Feature                | NPN                             | PNP                             |
|------------------------|---------------------------------|---------------------------------|
| Arrow direction        | Outward                         | Inward                         |
| Base voltage           | Higher than emitter             | Lower than emitter             |
| Current flow           | Collector → Emitter             | Emitter → Collector            |
| Common connection      | Emitter to GND                  | Emitter to +V                  |
| Typical use case       | Switching to ground             | Switching to positive supply   |

---

## 2. Features

* **Type:** NPN or PNP.
* **Gain (hFE):** Ratio of collector current to base current.
* **Maximum ratings:** Voltage (Vce), Current (Ic), Power (P).
* **Package:** TO-92, SOT-23, TO-220, etc.

## 4. How to Use
### Safety Note
Exceeding maximum ratings for voltage, current, or power can destroy the transistor.

### 4.1 Identify pins

- Use the datasheet : pin order varies between packages and manufacturers.
- Typical TO-92: **E-B-C** (Emitter, Base, Collector).

<img src="\images\2N4400-Pinout.jpg" width="500" height="300" alt="Transistor pinout">

### 4.2 Switching example (NPN)

For a 5V LED circuit:  
1. Connect **emitter to ground**.  
2. Connect **collector to LED**, LED to resistor, resistor to +5V.  
3. Apply small base current via a resistor from microcontroller.


### 4.3 Amplification example

- Small audio signal at base → larger output signal between collector and emitter.
- Requires proper **biasing resistors**.


### 4.4 Testing with a multimeter

- Use diode mode to check base-emitter and base-collector junctions.
- For NPN: Base to emitter & base to collector should show ~0.6–0.7V drop (forward).
- For PNP: Emitter to base & collector to base show ~0.6–0.7V drop.

## 5. Application

* Signal amplification.
* Switching (LEDs, motors, relays).
* Oscillator circuits.

## 6. Video Explanation
video coming soon 
