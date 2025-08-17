---
title: Pull-up/Pull-down Resistors
layout: home
parent: Basic Passive Components 
nav_order: 19
---

# Pull-up and Pull-down Resistors

## 1. Definition

### 1.1 Pull-up Resistor

A pull-up resistor is a resistor connected between a signal line and a positive voltage supply (Vcc).  
It ensures that the signal is at a logical **HIGH** level when no active device is driving it.

### 1.2 Pull-down Resistor

A pull-down resistor is a resistor connected between a signal line and ground (GND).  
It ensures that the signal is at a logical **LOW** level when no active device is driving it.


**symbols**

<img src="\images\pulluppulldown.jpg" width="500" height="300" alt="Pull-up and pull-down resistor symbols">



## 2. Features

* **Value Range:** typically from 1 kΩ to 100 kΩ.
* **Function:** sets a defined logic state when the input is floating.
* **Power Consumption:** higher resistance = less current draw, but slower response.
* **Internal vs External:** many microcontrollers have configurable internal pull-ups (or less commonly, pull-downs).
* **Voltage Rating:** must be compatible with the circuit logic voltage.



## 4. How to Use
### Safety Note
Incorrect resistor values can cause excessive current draw or unreliable logic levels, potentially damaging components or causing erratic behavior.


### 4.1. Identify if a pull-up/pull-down is needed

* Check if your input pin is **floating** when not connected, this can cause unpredictable behavior.
* Review datasheets: many ICs require external pull-ups or pull-downs for proper operation.



### 4.2. Choose the correct resistor value

* Common values: **4.7 kΩ** or **10 kΩ** for general-purpose logic circuits.
* Lower resistance → stronger pull, faster response, but more current draw.
* Higher resistance → weaker pull, slower response, but less current draw.



### 4.3. Connect it correctly

**Pull-up resistor:**
* Connect one side to the signal pin.
* Connect the other side to **Vcc**.

**Pull-down resistor:**
* Connect one side to the signal pin.
* Connect the other side to **GND**.


### 4.4. Test and verify

* Use a **multimeter** or logic analyzer to check voltage levels when the pin is not actively driven.
* Confirm that the default state is stable and doesn’t fluctuate.



### 4.5. Install in circuit

* ***On breadboard:*** insert between pin and Vcc (pull-up) or pin and GND (pull-down).
* ***On PCB:*** place close to the pin to reduce noise pickup.


## 5. When to Use

- **Microcontroller Inputs:** to prevent floating inputs from reading random values.
- **I²C Bus:** requires pull-up resistors on SDA and SCL lines for proper operation.
- **Switch Debouncing:** ensures defined logic level when switch is open.
- **Chip Enable Pins:** keeps device in a known state when not driven.
- **Reset Lines:** ensures proper startup state.



## 6. Video Explanation

video coming soon