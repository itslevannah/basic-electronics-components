---
title: Zener Diodes
layout: home
parent: Basic Active Components
nav_order: 22
---

# Zener Diodes


## 1. Definition
### 1.1 Zener Diode

A Zener diode is a special type of diode designed to allow current to flow in the forward direction like a normal diode, but also in the **reverse direction** when the voltage exceeds its specified **Zener breakdown voltage**.  
This makes it ideal for voltage regulation and reference applications.

<img src="\images\zenerdiodes.webp" width="500" height="300" alt="zener diode example">

**Zener diode symbol**

<img src="\images\symbol-1.png" width="500" height="300" alt="zener diode symbol">


### 1.2 Zener Breakdown Voltage

The **Zener breakdown voltage** (Vz) is the reverse voltage at which the diode begins to conduct in reverse without damage.  
Common values range from 2.4 V to over 200 V, depending on the diode design.



## 2. Features

* **Zener Voltage (Vz):** the regulated voltage the diode maintains under reverse breakdown.
* **Power Rating (Pz):** maximum power the diode can dissipate (Pz = Vz × Iz).
* **Reverse Current (Iz):** current flowing during breakdown mode.
* **Forward Voltage Drop (Vf):** ~0.7 V for silicon in forward bias.
* **Tolerance:** how close the actual breakdown voltage is to the rated value.
* **Package Type:** through-hole (DO-35, DO-41) or surface-mount (SOD-123, SOD-323).


## 4. How to Use
### Safety Note
Operating a Zener diode above its power rating will cause overheating and possible failure.  
Always use a current-limiting resistor in series when using it for voltage regulation.


### 4.1. Identify the Zener diode and polarity

* **Polarity:** cathode marked with a band, anode is the opposite lead.
* Markings often include the Zener voltage (e.g., “5V1” = 5.1 V).

<img src="\images\zener-diodemarking.jpg" width="500" height="300" alt="zener diode marking">


### 4.2. Choose the right Zener diode

* Select **Zener voltage** based on the desired regulated voltage.
* Ensure **power rating** is sufficient for the circuit.
* Consider **tolerance** for precision applications.


### 4.3. Connect it correctly

* **Reverse bias** for voltage regulation: cathode to positive, anode to ground.
* Use a **series resistor** to limit current.
* Can be placed in parallel with the load for shunt regulation.


### 4.4. Test and verify

* Use a power supply and resistor to measure breakdown voltage.
* Check that voltage across the Zener remains stable under varying load currents (within limits).


### 4.5. Install in circuit

* ***On breadboard:*** insert leads into holes, observing polarity.
* ***On PCB:*** solder into pads, matching the cathode band with the board marking.


## 5. When to Use

- **Voltage Regulation:** maintain a stable voltage for sensitive circuits.
- **Overvoltage Protection:** clamp excessive voltage to a safe level.
- **Voltage Reference:** provide a fixed reference in measurement systems.
- **Waveform Clipping:** limit signal peaks in audio and RF circuits.


## 6. Video Explanation

video coming soon