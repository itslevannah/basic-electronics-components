---
title: Debouncing
layout: home
parent: Prototyping & Circuit Building Tools
nav_order: 70
---


# Debouncing

## 1. Definition
**Debouncing** is A technique used to remove unwanted input noise from buttons, switches or other user input. Debouncing prevents extra activations or slow functions from triggering too often. 
Without debouncing, a single button press can register as multiple presses.

<img src="\images\Switch-Bouncing-in-the-Circuit.png" width="500" height="300" alt="Debouncing example">

---

## 2. Why Debouncing is Needed
When a **button** or **switch** is pressed, the contacts inside physically bounce for a few milliseconds.  
This causes the circuit to detect multiple signals instead of a single, clean one.  
Debouncing ensures **stable and reliable input**.

---

## 3. Types of Debouncing
### 3.1 Hardware Debouncing
- Uses resistors, capacitors, or dedicated ICs.  
- Filters out the bouncing signals before they reach the microcontroller.  
- More reliable for critical applications.  

### 3.2 Software Debouncing
- Done in code by adding a **delay** or logic that ignores repeated signals within a short time (e.g., 10–50 ms).  
- Easy to implement in Arduino or microcontrollers.  

---

## 4. Video Explanation
Video coming soon
