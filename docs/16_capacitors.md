---
title: Capacitors
layout: home
parent: Basic Passive Components 
nav_order: 16
---
# Capacitors
## 1 Definition
### 1.1 capacitor

A capacitor is a passive two-terminal electronic component that stores electrical energy in an electric field, created by a voltage difference between its plates.

<img src="\images\types-of-capacitors-.jpg" width="500" height="300" alt="capacitors"> 


**Capacitor symbol**

<img src="\images\capacitor-symbols-featured-1024x576.jpg" width="500" height="300" alt="Capacitor symbol"> 

### 1.2 Capasitence 
Capacitance is the ability of a substance or device to store an electrical charge.Commonly, capacitance is associated with capacitors.It is a measure of how much electric charge can be stored for a given voltage.

## 2. Features

* **Measurement:** measured in farads (F), typically in microfarads (µF), nanofarads (nF), or picofarads (pF).
* **Voltage Rating:** maximum voltage it can safely handle without breaking down.
* **Tolerance:** how much the actual capacitance can vary from the stated value (e.g., ±5%, ±10%, ±20%).
* **Temperature Coefficient:** capacitance changes with temperature.
* **Physical Size:** larger capacitors often have higher capacitance or voltage ratings.
* **Fixed or Variable:** can be fixed (most common) or adjustable (trimmer capacitors).


## 4. How to Use
### Safety Note
 Do not touch the terminals of a charged capacitor. Capacitors can store a dangerous electric charge even after power is disconnected,  which may result in electric shock.

### 4.1. Identify the capacitor value

* Read printed numbers (e.g., “104” = 100 nF) or use a capacitance meter.
* Value is given in Farads (F) or its smaller units (µF, nF, pF).

<img src="\images\capacitor-tantalum-leaded-markings-1542.jpg" width="500" height="300" alt="capacitor value code">  



### 4.2. Choose the right capacitor

* **Capacitance value** (for filtering, timing, or coupling needs).
* **Voltage rating** (must be higher than the circuit voltage).
* **Type** (electrolytic, ceramic, film, tantalum, etc.).


### 4.3. Connect it correctly

* **Polarity:** electrolytic and tantalum capacitors are polarized (marked with + or –); ceramic capacitors are non-polarized.
* In ***parallel***: total capacitance is the sum of all capacitors.
  **=>** increases overall capacitance.
* In ***series***: total capacitance is less than the smallest capacitor.
  **=>** increases overall voltage handling, decreases capacitance.


### 4.4. Test and verify

* Use a ***multimeter with capacitance mode*** to measure actual capacitance.
* Check for **leakage current** in electrolytics.
* Ensure the capacitor is not overheating or bulging.


### 4.5. Install in circuit

* ***On breadboard***: insert leads into holes.
* ***On PCB***: solder into the correct pads, respecting polarity.

## 5. When to use

- **Energy Storage:** to store and release electrical energy quickly (e.g., camera flash).  
- **Filtering:** to smooth voltage in power supplies by reducing ripple.  
- **Coupling/Decoupling:** to block DC and allow AC signals in audio or communication circuits, or to stabilize voltage.  
- **Timing Circuits:** with resistors to set delays or oscillation frequencies.
- **Filtering in AC to DC Circuits**: Capacitors smooth the pulsating DC output from a rectifier, making it closer to a steady DC voltage.
## 6. Video Explanation

video coming soon


