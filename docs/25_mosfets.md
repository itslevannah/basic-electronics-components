---
title: MOSFETs
layout: home
parent: Basic Active Components
nav_order: 25
---

# Metal-Oxide-Semiconductor Field-Effect Transistors (MOSFETs)

## 1. Definition
### 1.1 MOSFET

A **MOSFET** (Metal–Oxide–Semiconductor Field-Effect Transistor) is an electronic switch or amplifier.  
Unlike a regular transistor (BJT), it is controlled by **voltage** at its gate terminal instead of current.  
This makes it very efficient ; it can switch large currents with almost no power used to control it.

It has three main pins:
- **Gate (G):** Controls the switch.
- **Drain (D):** Current flows **out** here in N-channel (or into here in P-channel).
- **Source (S):** Current flows **in** here in N-channel (or out here in P-channel).

<img src="\images\MOSFET Symbol.webp" width="500" height="300" alt="MOSFET examples">

**MOSFET Symbols**

<img src="\images\images.png" width="500" height="300" alt="MOSFET symbols">



### 1.2 N-Channel vs P-Channel MOSFETs

#### **N-Channel MOSFET**
- **Symbol:** Arrow points **in** to the source.
- **Operation:** Turns on when **gate voltage is higher than source**.
- **Current flow:** Drain → Source.
- **Common use:** Low-side switching (connect source to ground).

#### **P-Channel MOSFET**
- **Symbol:** Arrow points **out** from the source.
- **Operation:** Turns on when **gate voltage is lower than source**.
- **Current flow:** Source → Drain.
- **Common use:** High-side switching (connect source to positive supply).

**Side-by-side comparison:**

| Feature                | N-Channel                       | P-Channel                       |
|------------------------|---------------------------------|----------------------------------|
| Arrow direction        | Into source                     | Out from source                  |
| Gate voltage to turn on| Higher than source               | Lower than source                |
| Current flow           | Drain → Source                  | Source → Drain                   |
| Common connection      | Source to GND                   | Source to +V                     |
| Typical use case       | Switching ground                | Switching positive supply        |



## 2. Features

* **Type:** N-channel or P-channel.
* **Logic-level or standard gate drive:** Logic-level MOSFETs can be driven directly by microcontrollers (e.g., 5V or 3.3V).
* **RDS(on):** Resistance when on , lower is better for efficiency.
* **Max current and voltage ratings.**
* **Package:** TO-220, TO-92, SMD types.



## 4. How to Use
### Safety Note
MOSFET gates are sensitive to static electricity; always discharge yourself before touching pins.



### 4.1 Identify the pinout

- Check the datasheet : pin order varies.
- Common TO-220 pin order: **Gate , Drain , Source**.

<img src="\images\P55NF06-Pinout.jpg" width="500" height="300" alt="MOSFET pinout">



### 4.2 Switching example (N-channel)

To control an LED strip from an Arduino:
1. Connect **source to ground**.
2. Connect **drain to LED strip negative**.
3. Connect LED strip positive to +12V.
4. Connect Arduino pin to gate through a 100Ω resistor.
5. Add a 10kΩ resistor from gate to ground (keeps it off when not driven).



### 4.3 Switching example (P-channel)

To switch +12V to a device:
1. Connect **source to +12V**.
2. Connect **drain to device positive**.
3. Connect device negative to ground.
4. Pull gate **low** (below source voltage) to turn on, **high** to turn off.



### 4.4 Testing with a multimeter

- Set meter to diode mode.
- For N-channel:  
  - Check **drain to source** , should be open when gate is uncharged.
  - Briefly touch gate to source to discharge.  
  - Apply small voltage between gate and source , drain-source path becomes conductive.
- For P-channel: reverse polarities for the same test.



## 5. Applications

* Driving motors, LEDs, relays.
* High-efficiency power supplies.
* Battery protection circuits.
* Logic-level signal switching.

## 6. Video Explanation
video coming soon