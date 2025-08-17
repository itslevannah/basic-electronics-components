---
title: Servos
layout: home
parent: Electromechanical Components
nav_order: 33
---

# Servo Motors

## 1. Definition
### 1.1 Servo Motor

A servo motor is a **DC motor with gears, a sensor, and a small controller inside** that allows it to move to and hold a specific angle.  


Common hobby servos rotate 0° to 180°, while **continuous rotation servos** act more like geared DC motors (they keep spinning).

<img src="\images\Servo Motor.jpg" width="500" height="300" alt="Servo Motor example">


**Servo Symbol**

<img src="\images\Schematic-diagram-and-pinout-of-a-servo-motor-vi-DC-motor.jpg" width="500" height="300" alt="Servo symbol">


### 1.2 Types of Servos

- **Positional Rotation:** Limited to a fixed range (e.g., 0° to 180°).
- **Continuous Rotation:** Spins freely in either direction (speed controlled by PWM).
- **Linear Servos:** Move back and forth in a straight line instead of rotating.


## 2. Features

* Controlled by a **PWM (Pulse Width Modulation) signal**.
* Built-in gearing for higher torque.
* Internal feedback system for accurate positioning.
* Typical operating voltage: **4.8V to 6V** (some up to 7.4V for high-performance models).
* Torque (strength) & speed vary by model **_check datasheets before use._**


## 4. How to Use
### Safety Note
Never force the servo horn by hand, you can strip the internal gears.



### 4.1 Wiring

* **Brown or Black:** Ground (GND)  
* **Red:** Power (Vcc)  
* **Orange or Yellow:** PWM control signal (connect to Arduino PWM pin, e.g., pin 9)

<img src="\images\servo_pinout.jpg" width="500" height="300" alt="Servo pinout">



### 4.2 Controlling

* Send a short **pulse** every 20ms to set the angle:
  - **1ms pulse → 0°** (full left)
  - **1.5ms pulse → 90°** (center)
  - **2ms pulse → 180°** (full right)

* _Arduino makes this easy_ using the built-in **Servo library**:  


## Video Explanation
video coming soon