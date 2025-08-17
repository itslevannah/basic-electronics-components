---
title: Voltage Regulators
layout: home
parent: Power Sources & Protection
nav_order: 38
---

# Voltage Regulators

## 1. Definition
### 1.1 Voltage Regulator

A voltage regulator is an electronic component that keeps the output voltage steady, even if the input voltage changes or the load varies.  
They are used to protect circuits from voltage fluctuations and ensure reliable operation.

<img src="\images\Voltage-regulators.jpg" width="500" height="300" alt="Voltage regulator examples">

**Voltage Regulator Symbol**

<img src="\images\Voltage-Regulator-IEC-Symbol.svg.png" width="500" height="300" alt="Voltage regulator symbol">


### 1.2 Types of Voltage Regulators

- **Linear Regulators**  Simple, low noise, but less efficient. Example: **7805** (5V fixed output).
- **Adjustable Regulators**  Output set by external resistors. Example: **LM317**.
- **Switching Regulators**  High efficiency, can step voltage up or down (buck, boost, buck-boost).

 **Beginner Tip:**  
Use **linear regulators** when efficiency isn’t critical and the voltage drop is small.  
Use **switching regulators** for battery-powered or high-current applications.


## 2. Features

* **Output type:** Fixed or adjustable.
* **Maximum output current**  don’t exceed this limit.
* **Efficiency**  important for battery life.
* **Dropout voltage**  minimum difference between input and output for proper regulation.


## 4. How to Use
### Safety Note
Linear regulators can get **very hot** if the voltage drop and current are large, plan for heatsinking.


### 4.1 Identify Pins

Example: **7805** (front view, pins downwards)  
1. **Input (Vin)**  higher than desired output.  
2. **Ground (GND)**.  
3. **Output (Vout)**  regulated voltage.

<img src="\images\LM7806-Pinout.jpg" width="500" height="300" alt="Voltage regulator pinout">



### 4.2 Example Power Loss Calculation

If **Vin = 12V**, **Vout = 5V**, **load current = 1A**:  
Heat dissipated = (12V − 5V) × 1A = **7W**.  
This means the regulator will convert 7 watts into heat, a heatsink is strongly recommended.


### 4.3 Common Applications

* Powering microcontrollers from batteries or adapters.
* Providing a stable reference voltage for sensors.
* Regulating voltage in battery charging circuits.



### 4.4 Common Beginner Mistakes

* Reversing the pinout, always check the datasheet.
* Forgetting the dropout voltage , regulator may not work if input is too low.
* Ignoring heat dissipation , can cause thermal shutdown or failure.

## 5. Video Explanation
video coming soon