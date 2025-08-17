---
title: Inductors
layout: home
parent: Basic Passive Components 
nav_order: 17
---

# Inductors


## 1. Definition
### 1.1 Inductor

An inductor is a passive two-terminal electronic component that stores energy in a magnetic field when electric current flows through it. It usually consists of a coil of wire wound around a core, which may be air, ferrite, or iron.

<img src="\images\types of inductors.jpg" width="500" height="300" alt="types of inductors"> 

**Inductor symbol**

<img src="\images\Inductor_symbol.png" width="500" height="300" alt="Inductor symbol"> 

### 1.2 Inductance

Inductance is the property of an electrical conductor to oppose a change in current by generating a voltage (EMF) proportional to the rate of current change.  
It is measured in **henries (H)**, typically in millihenries (mH) or microhenries (µH).


## 2. Features

* **Measurement:** in henries (H), usually mH or µH for practical circuits.
* **Current Rating:** maximum continuous current without overheating.
* **DC Resistance (DCR):** resistance of the wire; lower DCR means higher efficiency.
* **Saturation Current:** the current at which the core material stops storing additional magnetic energy effectively.
* **Core Material:** affects performance (air core for high-frequency, ferrite or iron core for power applications).
* **Tolerance:** variation from stated inductance value.
* **Physical Size:** larger inductors can handle more current and have higher inductance.


## 4. How to Use
### Safety Note
While inductors don’t store charge like capacitors, they can generate **high voltage spikes** when current is suddenly interrupted. This can damage components or cause electric shock in certain cases. Please handle switching circuits with care.


### 4.1. Identify the inductor value

* Look for printed markings or color codes, or use an **LCR meter**.
* Values are given in henries (H), millihenries (mH), or microhenries (µH).

<img src="\images\inductor-color-codes.jpg" width="500" height="300" alt="inductor value code">  


### 4.2. Choose the right inductor

* **Inductance value** (determines filtering, timing, or energy storage behavior).
* **Current rating** (must exceed the maximum current in the circuit).
* **Core type** (air, ferrite, iron powder, laminated steel, etc.).
* **Frequency range** (some inductors are optimized for high-frequency RF, others for low-frequency power).


### 4.3. Connect it correctly

* Inductors are **non-polarized**  they can be connected in either direction.
* In ***series***: total inductance is the sum of all inductors.
  **=>** increases overall inductance.
* In ***parallel***: total inductance is less than the smallest inductor.
  **=>** decreases overall inductance, increases current handling.


### 4.4. Test and verify

* Use an **LCR meter** to measure inductance.
* Check **DCR** to ensure efficiency.
* In switching circuits, check for excessive heating.


### 4.5. Install in circuit

* ***On breadboard***: insert leads into holes.
* ***On PCB***: solder into the correct pads, keeping them away from sensitive signal traces if high currents are involved.


## 5. When to Use

- **Filtering:** with capacitors to create LC filters in power supplies and signal processing.
- **Energy Storage:** in switch-mode power supplies to store and transfer energy.
- **Chokes:** to block high-frequency AC while allowing DC or low-frequency AC to pass.
- **Tuning Circuits:** in radio transmitters and receivers to select specific frequencies.
- **Transformers:** as part of coupled inductors to step up or step down voltages.


## 6. Video Explanation

video coming soon