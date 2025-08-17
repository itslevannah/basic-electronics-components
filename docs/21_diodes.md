---
title: Diodes
layout: home
parent: Basic Active Components
nav_order: 21
---

# Diodes

## 1. Definition
### 1.1 Diode

A diode is a two-terminal semiconductor device that allows current to flow in one direction only, blocking it in the opposite direction.  
It is used for rectification, protection, and signal control in electronic circuits.

**What is a semiconductor**
A semiconductor is a material whose ability to conduct electricity falls between that of a conductor (like copper) and an insulator (like glass).

<img src="\images\Types-of-Diodes-with-Symbol.jpg" width="500" height="300" alt="types of diodes">

**Diodes symbols**

<img src="\images\diodes symbol.jpg" width="500" height="300" alt="diode symbol">

**Cathode Vs. Anode**

In an LED, the cathode is the negative terminal (typically the shorter lead and the side with a flat edge on the casing), while the anode is the positive terminal (typically the longer lead). In other diodes, the cathode is usually marked with a band, and the anode is the opposite end.

<img src="\images\cathodepola.webp" width="500" height="300" alt="cathode marking symbol">

**Polarity Marking in Different Diodes**

<img src="\images\cathodepolaritymarking.png" width="500" height="300" alt="cathode marking symbol">


### 1.2 Forward and Reverse Bias

- **Forward bias:** current flows when the anode is at a higher voltage than the cathode, and the voltage exceeds the diode’s forward voltage drop (typically 0.7 V for silicon, 0.3 V for germanium).
- **Reverse bias:** current is blocked when the cathode is at a higher voltage than the anode, up to the diode’s breakdown voltage.


## 2. Features

* **Forward Voltage Drop (Vf):** voltage needed for the diode to conduct (e.g., 0.7 V for silicon, ~0.2–0.3 V for Schottky).
* **Maximum Forward Current (If):** maximum continuous current the diode can handle.
* **Reverse Breakdown Voltage (Vbr):** voltage at which the diode will conduct in reverse.
* **Reverse Leakage Current:** small current that flows under reverse bias.
* **Recovery Time:** important in high-speed switching applications.
* **Package Type:** through-hole (DO-41, DO-35) or SMD.


## 4. How to Use
### Safety Note
Connecting a diode in reverse beyond its breakdown voltage can permanently damage it (except in Zener diodes, where breakdown is intended).


### 4.1. Identify the diode type and polarity

* **Polarity:** the **cathode** is usually marked with a band; the other lead is the **anode**.
* Common types: **Rectifier, Schottky, Zener, Light Emitting Diode (LED), Photodiode**.

<img src="\images\diode-polarity.jpg" width="500" height="300" alt="diode polarity marking">



### 4.2. Choose the right diode

* **Application:** rectification, voltage regulation, signal detection, light emission, etc.
* **Current rating** (must be higher than circuit current).
* **Reverse voltage rating** (must be higher than maximum reverse voltage in circuit).
* **Speed:** for high-frequency circuits, use fast recovery or Schottky diodes.



### 4.3. Connect it correctly

* **Series connection:** to allow current in one direction only.
* **Parallel (reverse) connection:** for polarity protection.
* Observe correct polarity ; anode to positive, cathode to negative (unless using a Zener in reverse mode).



### 4.4. Test and verify

* Use the **diode test mode** on a multimeter to measure forward voltage drop.
* Check that it blocks current in reverse direction under normal conditions.
* For LEDs, test with low current to avoid damage.



### 4.5. Install in circuit

* ***On breadboard:*** insert leads into holes, observing polarity.
* ***On PCB:*** solder into the correct orientation according to PCB silkscreen markings.


## 5. When to Use

- **Rectification:** converting AC to DC in power supplies.
→ standard rectifier diodes (1N4007, etc.)
- **Reverse Polarity Protection:** prevent damage from wrong power connection.
→ general-purpose or Schottky diodes
- **Voltage Regulation:** Zener diodes for fixed voltage reference.
→ Zener diodes
- **Signal Demodulation:** in AM/FM radio circuits.
→ small-signal diodes (1N4148, etc.)
- **Switching:** in high-speed logic and RF circuits.
→ fast-recovery, Schottky, or PIN diodes
- **Light Emission/Detection:** LEDs and photodiodes.
→ LEDs and photodiodes


## 6. Video Explanation

video coming soon