---
title: LEDs
layout: home
parent: Basic Active Components
nav_order: 23
---

# Light Emitting Diodes (LEDs)

## 1. Definition
### 1.1 LED

A Light Emitting Diode (LED) is a semiconductor device that emits light when an electric current passes through it.  
Unlike incandescent bulbs, LEDs produce light by **electroluminescence**, where electrons recombine with holes in the semiconductor material, releasing energy in the form of photons.

<img src="\images\SMALLLEDBULB.webp" width="500" height="300" alt="LED examples">

**LED Explained**

<img src="\images\ledexplained.webp" width="500" height="300" alt="LED Explained">

**LED symbol**

<img src="\images\ledsymbol.png" width="500" height="300" alt="LED symbol">


### 1.2 LED Colors and Materials

The color of an LED depends on the semiconductor material and the energy gap:
- **Red, Yellow, Green:** typically made from gallium arsenide phosphide (GaAsP) or gallium phosphide (GaP).
- **Blue, White:** often made from gallium nitride (GaN).
- **Infrared:** gallium arsenide (GaAs).

**Infrared LED**
<img src="\images\infrared led.jpg" width="500" height="300" alt="LED Infrared">

## 2. Features

* **Forward Voltage (Vf):** usually 1.8–3.3 V depending on color.
* **Forward Current (If):** typically 10–20 mA for standard LEDs.
* **Light Intensity:** measured in millicandela (mcd) or lumens.
* **Viewing Angle:** determines the spread of emitted light.
* **Polarity Sensitive:** will not light if connected backwards.
* **Colors & Types:** single-color, RGB, infrared, UV, high-power, and indicator LEDs.


## 4. How to Use
### Safety Note
LEDs must be used with a **current-limiting resistor** or constant current driver to prevent damage.


### 4.1. Identify LED polarity

* **Cathode (negative):** typically the shorter lead, flat spot on the rim, or larger internal electrode.
* **Anode (positive):** longer lead and smaller internal electrode.

<img src="\images\led-polarity.jpg" width="500" height="300" alt="LED polarity">


### 4.2. Choose the right LED

* Select **color/wavelength** based on application.
* Match **forward voltage** and **current** to the driver circuit.
* Choose intensity and viewing angle for visibility needs.


### 4.3. Connect it correctly

* Connect **anode to positive**, **cathode to ground** through a resistor.
* Calculate resistor value:  

**R = Vsupply - Vf / If**

Example: For 5 V supply, red LED (Vf = 2 V), If = 20 mA:  
R = 5-2 / 0.02 = 150 Ω

### 4.4. Test and verify

* Use a multimeter’s **diode test mode** to check polarity and function.
* LED should light dimly under diode test (forward bias).


### 4.5. Install in circuit

* ***On breadboard:*** insert leads in*

## 5. Video Explanation
video coming soon