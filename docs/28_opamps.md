---
title: Operational Amplifiers (Op-Amps)
layout: home
parent: Basic Active Components
nav_order: 28
---

# Operational Amplifiers (Op-Amps)

## 1. Definition
### 1.1 What is an Op-Amp?

An **Operational Amplifier**, or **Op-Amp**, is a special kind of electronic chip that can make weak signals much stronger.  
It has **two inputs** and **one output**, and it compares the voltages at the inputs.

Think of it like a “volume knob” for voltage, it can amplify tiny voltages from a microphone, sensor, or antenna so other circuits can use them.

<img src="\images\Ua741_opamp.jpg" width="500" height="300" alt="Op-Amp examples">

**Op-Amp Symbol**

<img src="\images\Op-amp_symbol.svg.png" width="500" height="300" alt="Op-Amp symbol">



### 1.2 Common Op-Amp ICs

- **LM741** : classic, general-purpose op-amp.  
- **TL081** : low-noise op-amp, good for audio.  
- **LM358** : dual op-amp, works well with low voltage.


## 2. Features

* **High input impedance** : doesn’t load down the signal source.  
* **Low output impedance** : can drive the next stage easily.  
* **Very high voltage gain** : can amplify signals thousands of times.  
* Can be set up for many jobs: amplification, filtering, comparing voltages, etc.



## 4. How to Use
### Safety Note
Never apply a voltage higher than the op-amp’s power supply.  
Doing so can damage the chip.



### 4.1 Pin functions (LM741 example)

1. **Offset Null (-)** : Fine adjustment for perfect zero output.  
2. **Inverting Input (-)** : Signal here is amplified but inverted (flipped).  
3. **Non-inverting Input (+)** : Signal here is amplified without inversion.  
4. **V-** : Negative supply voltage (or ground in single-supply circuits).  
5. **Offset Null (+)** : Fine adjustment.  
6. **Output** : Amplified signal comes out here.  
7. **V+** : Positive supply voltage.  
8. **NC** : No internal connection.



### 4.2 Basic Inverting Amplifier Example

If you connect an op-amp with two resistors like this:

- **Rin** between your signal and the inverting input (-)  
- **Rf** between output and inverting input (-)  
- Non-inverting input (+) connected to ground

The **gain** (how much it amplifies) is:


Gain = - Rf/Rin

Example:  
- Rin = 10 kΩ  
- Rf = 100 kΩ  
- Gain = -10 (signal is 10× bigger and inverted)


### 4.3 Common Applications

* **Audio amplifiers** : boost microphone or guitar signals.  
* **Filters** : remove noise or unwanted frequencies.  
* **Comparators** : detect when one voltage is higher than another.  
* **Signal conditioning** : prepare sensor signals for a microcontroller.

## 5. Video Explanation
video coming soon