---
title: Motors (DC/Stepper)
layout: home
parent: Electromechanical Components
nav_order: 32
---

# Motors (DC & Stepper)

## 1. Definition
### 1.1 DC Motor

A DC motor converts electrical energy into mechanical rotation using direct current.  
**_Think of it as an electric fan without the blades,  give it power, and the shaft spins._**

<img src="\images\voltaat-motors-motors-fans-small-brushed-dc-motor-5v-16500-rpm-with-jumper-wires-1125737655_1024x1024.webp" width="500" height="300" alt="DC Motor example">



### 1.2 Stepper Motor

A stepper motor moves in **discrete steps**, providing precise control over position without feedback.  
**_Instead of spinning freely like a DC motor, it moves in tiny fixed jumps, perfect for positioning systems._**

<img src="\images\stepper-motor-cm-series-86cm45c-standard-leadshine-india-760160.webp" width="500" height="300" alt="Stepper Motor example">



**Motor Symbols**

<img src="\images\qe0XG.jpg" width="500" height="300" alt="Motor symbols">

**_The circles with “M” are generic motors, while the segmented circle often represents a stepper._**



## 2. Features

* **DC Motors:** Simple speed control via voltage or PWM (Pulse Width Modulation). **_(More voltage = faster spin.)_**
* **Stepper Motors:** Controlled via step pulses for exact positioning. **_(Number of pulses = how far it moves.)_**
* Voltage & current ratings. **_(Match these to your power supply to avoid burning the motor.)_**
* Torque & speed specs. **_(Torque = how strong it is; speed = how fast it spins.)_**


## 4. How to Use
### Safety Note
Motors can draw **high startup current**; ensure your driver circuit supports it.  
**_(A motor can briefly pull several times its normal current when starting, this can fry weak drivers.)_**



### 4.1 Identify terminals

* **DC Motor:** Two terminals. Reversing polarity reverses rotation.
* **Stepper Motor:** Multiple coils (4, 5, 6, or 8 wires).  
  **_(More wires = more coil configurations. Datasheet tells you which is which.)_**



### 4.2 Driving motors

* **DC motor:** Use an H-bridge or motor driver IC. **_(Like the L293D or L298N.)_**
* **Stepper motor:** Use a dedicated stepper driver (e.g., A4988, DRV8825) to send step pulses.



### 4.3 Applications

* Robotics (wheel drive, arm movement).
* CNC machines (precise positioning).
* Fans and pumps (continuous rotation).

**_Common beginner project: Use Arduino to control a DC motor with a potentiometer for speed, or a stepper motor to turn a dial to a set angle._**

## 5. Video Explanation
video coming soon