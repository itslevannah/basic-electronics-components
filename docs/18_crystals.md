---
title: Crystal Oscillators
layout: home
parent: Basic Passive Components 
nav_order: 18
---

# Crystal Oscillators

## 1. Definition
### 1.1 Crystal Oscillator

A crystal oscillator is an electronic device that uses the mechanical resonance of a vibrating crystal (typically quartz) to generate a precise and stable frequency signal.  
It is commonly used for clock generation in microcontrollers, communication systems, and timing applications.

<img src="\images\crystal oscillator.jpg" width="500" height="300" alt="crystal oscillators">

**Crystal oscillator symbol**

<img src="\images\crystal oscillator symbol.png" width="500" height="300" alt="crystal oscillator symbol">

**Crystal oscillator Circuit**
Schematic symbol and equivalent circuit for a quartz crystal in an oscillator

<img src="\images\cryastaloscillator components.png" width="500" height="300" alt="crystal oscillator symbol">

### 1.2 Resonant Frequency

The resonant frequency is the frequency at which the crystal naturally vibrates when an electrical signal is applied.  
It is determined by the crystal’s **cut, shape, and size** and is measured in **hertz (Hz)**, typically in kHz or MHz for practical use.


## 2. Features

* **Frequency Range:** most common are 32.768 kHz (for real-time clocks) and several MHz (for microcontrollers).
* **Frequency Stability:** how much the output drifts with temperature, load, or aging.
* **Load Capacitance:** external capacitance needed to achieve the specified frequency.
* **Drive Level:** the amount of power applied to the crystal, usually measured in microwatts.
* **Aging Rate:** slow change in frequency over time.
* **Package Type:** through-hole (metal can) or SMD (surface mount).


## 4. How to Use
### Safety Note
Crystals are physically delicate; excessive mechanical shock, bending, or overheating during soldering can damage them.  
Also, driving a crystal beyond its rated power can crack it internally.


### 4.1. Identify the crystal oscillator

* Frequency is usually printed on the metal can or package (e.g., **8.000 MHz**, **32.768 kHz**).
* Package style can help identify the mounting method (e.g., HC-49, SMD).

<img src="\images\crystal-markings.jpg" width="500" height="300" alt="crystal markings">


### 4.2. Choose the right crystal oscillator

* **Frequency** (must match the circuit’s design requirements).
* **Load capacitance** (specified in the datasheet; match with circuit capacitors).
* **Stability** (ppm rating, e.g., ±20 ppm).
* **Package type** (through-hole or surface-mount).
* **Temperature range** (especially for outdoor or industrial use).


### 4.3. Connect it correctly

* Crystals are **non-polarized**, so orientation doesn’t matter electrically.
* Usually connected across the input and output pins of an oscillator circuit, with capacitors to ground.
* For microcontrollers: connect to the XTAL pins and follow datasheet capacitor recommendations.


### 4.4. Test and verify

* Use an **oscilloscope** or **frequency counter** to confirm output frequency.
* Ensure proper oscillation startup, incorrect load capacitors can prevent operation.
* Check for drift with temperature if stability is critical.


### 4.5. Install in circuit

* ***On breadboard:*** not recommended for high-frequency crystals due to stray capacitance.
* ***On PCB:*** keep leads short and capacitors close to reduce noise and instability.


## 5. When to Use

- **Microcontroller Clock Source:** to provide precise timing for CPUs.
- **Real-Time Clocks (RTC):** 32.768 kHz crystals for low-power timekeeping.
- **Communication Systems:** for frequency generation in transmitters and receivers.
- **Signal Processing:** as part of frequency synthesizers and filters.
- **Test Equipment:** in frequency standards.



## 6. Video Explanation

video coming soon