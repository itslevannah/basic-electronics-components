---
title: Kirchhoff’s Voltage Law (KVL)
layout: home
parent: Core Theory & Laws of Electronics
nav_order: 6
---

# Kirchhoff’s Voltage Law (KVL)

## 1. Definition
Kirchhoff’s second law, or Kirchhoff’s loop rule, states that the **sum of all voltages around any closed loop in a circuit is equal to zero**.  
This means the total voltage rises are equal to the total voltage drops in that loop.  
It is based on the **principle of conservation of energy**.

---

### 1.1. Visualization

<img src="\images\Kirchhoff_voltage_law.svg.png" width="500" height="300" alt="KVL Example">

- *The sum of all the voltages around a loop is equal to zero.*
v1 + v2 + v3 + v4 = 0
- When you go around a closed circuit loop, every increase in electric potential **(voltage rise)** is balanced by a decrease in electric potential **(voltage drop)**.
- The algebraic sum of voltages in a closed loop is zero.


### 1.2. In Formula Form
Sum of Voltage Rises; Sum of Voltage Drops = 0

Or equivalently:

Sum of Voltages = 0

Where:  
- V = Voltage (in volts, V)  
- The sign of V depends on whether you move from the negative to positive terminal (rise) or from positive to negative terminal (drop).



### 1.3. Example

Consider a simple loop with a 12 V battery and two resistors with voltage drops of 7 V and 5 V:

12 - 7 - 5 = 0

KVL confirms the loop is balanced because the total sum is zero.


## 2. Usage

- Calculating unknown voltages in a circuit.
- Verifying that a circuit is wired correctly.
- Analyzing multi-loop circuits with **mesh analysis**.
- Troubleshooting voltage drops in wiring or components.


## 3. Limitations

- Assumes **steady-state DC** or low-frequency AC circuits where inductive and capacitive effects are negligible.
- For high-frequency circuits, parasitic inductance and capacitance can cause small deviations from the law.
- Requires a clearly defined loop and consistent sign convention for rises and drops.


## 4. Video Explanation
video coming soon