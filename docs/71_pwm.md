---
title: PWM (Pulse Width Modulation)
layout: home
parent: Prototyping & Circuit Building Tools
nav_order: 71
---


# Pulse Width Modulation (PWM)

## 1. Definition
**PWM (Pulse Width Modulation)** is a technique used to control the amount of power delivered to electronic devices.  
Instead of changing voltage directly, it rapidly switches the signal **ON and OFF** at high speed, and the ratio of ON-time to OFF-time determines the effective output.

<img src="\images\pulse-width-modulation_01.jpg" width="500" height="300" alt="PWM signal example">

**Duty Cycle:** The percentage of time the signal is ON compared to the total cycle time.  
- 0% Duty Cycle → Always OFF  
- 50% Duty Cycle → ON half the time  
- 100% Duty Cycle → Always ON  



## 2. Applications
- **LED Dimming:** Control brightness smoothly.  
- **Motor Control:** Adjust speed without extra heating.  
- **Sound Generation:** Create tones using different frequencies.  
- **Power Regulation:** Efficient control of voltage and power to devices.  


## 3. How it Works
- A **digital pin** switches between HIGH (ON) and LOW (OFF).  
- The switching happens very fast (thousands of times per second).  
- The device (LED, motor, etc.) perceives it as a variable power level instead of flickering.  


## 4. Video Explanation
Video coming soon