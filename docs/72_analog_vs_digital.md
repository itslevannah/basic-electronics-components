---
title: Analog vs Digital Signal
layout: home
parent: Prototyping & Circuit Building Tools
nav_order: 67
---



# Analog vs Digital Signals

## 1. Definition
In electronics, signals are how information (like sound, light, or data) is represented and transferred.  
There are **two main types of signals**: **Analog** and **Digital**.

- **Analog Signals**: Continuous values (smooth waveforms).  
- **Digital Signals**: Discrete values (steps, usually 0s and 1s).



## 2. Analog Signals
- Vary **continuously** over time.  
- Can take **infinite values** within a range.  
- Examples: sound from a microphone, light intensity, temperature.  

**Visual Example:**  
A smooth sine wave curve.
<img src="\images\1_33.png" width="500" height="300" alt="PWM signal example">



## 3. Digital Signals
- Represented in **discrete steps** (0 or 1, HIGH or LOW).  
- More reliable for computers and microcontrollers.  
- Examples: ON/OFF switch, binary data, PWM control signals.  

**Visual Example:**  
A square wave (only HIGH and LOW levels).

<img src="\images\digital_signal.jpg" width="500" height="300" alt="PWM signal example">


## 4. Key Differences

| Feature            | Analog                         | Digital                   |
|--------------------|--------------------------------|---------------------------|
| Values             | Continuous (infinite)          | Discrete (0/1)            |
| Signal Shape       | Smooth (sine wave)             | Square (steps)            |
| Example            | Temperature, sound, light      | Switches, microcontrollers|
| Noise Sensitivity  | More sensitive to noise        | Less sensitive            |



## 5. Applications
- **Analog**: Music, sensors (temperature, light, sound).  
- **Digital**: Computers, microcontrollers (Arduino, Raspberry Pi).  



## 6. Safety Note
Always check if your circuit needs **analog input (A0 pin)** or **digital input/output (D0–Dx pins)** on Arduino/boards, to avoid wiring mistakes.

## 7. Video Explanation
Video coming soon