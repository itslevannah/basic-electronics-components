---
title: Kirchhoff’s Current Law (KCL)
layout: home
parent: Core Theory & Laws of Electronics
nav_order: 5
---

# Kirchhoff’s Current Law (KCL)
## 1. Definition   
Kirchhoff's first law, or Kirchhoff's junction rule, states that, for any node (junction) in an electrical circuit, **the sum of currents flowing into that node is equal to the sum of currents flowing out of that node.**

## 1.1. Visualization

<img src="\images\KCL_-_Kirchhoff's_circuit_laws.svg.png" width="500" height="300" alt="KCL">

- *The current entering any junction is equal to the current leaving that junction :* \[i2 + i3 = i1 + i4\]
-  The sum of currents entering and leaving a junction, with currents entering counted as positive and leaving as negative, always equals zero.

### 1.2. In Formula Form
<img src="\images\592ac33b15e395ad2bdccdb57bebf8ddc67945c8.svg" width="500" height="300" alt="Formula of KCL">

or Equivalently :
**Sum of currents in = Sum of currents out**

Where:
- I = Current is measured in amperes (A).
- n = the total number of branches with currents flowing towards or away from the node. 

### 1.3. Example

If 4A and 2A flow into a junction, and one branch has 3A flowing out, the other branch must have:
I out = 4+2−3 =3A

So the total is zero: 

4A + 2A - 3A -3A = 0A

## 2. Usage
- Calculating unknown currents in a circuit.
- Analyzing complex networks of resistors, capacitors, or other components.
- Circuit troubleshooting to detect wiring or component faults.
- Ensuring correct current distribution in power systems.

## 3. Limitations

- KCL assumes steady state conditions (currents are constant over time), for rapidly changing fields, displacement currents must be considered.

- Assumes ideal conductors with no charge storage at junctions.

- In very high-frequency AC circuits, stray capacitance or inductance can cause small deviations.

## 4. Video Explanation 
video coming soon