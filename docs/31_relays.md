---
title: Relays
layout: home
parent: Electromechanical Components
nav_order: 31
---

# Relays

## 1. Definition
### 1.1 Relay

A relay is an electromechanical switch that uses an electromagnetic coil to open or close contacts in another circuit.  
It allows **low-power control signals** to operate **high-power devices**.  


<img src="\images\electronic-relay-500x500.webp" width="500" height="300" alt="Relay examples">

**Relay Symbol**

<img src="\images\imagesrelay.png" width="500" height="300" alt="Relay symbol">

**_The symbol shows the coil (control side) and the contacts (switching side). They’re separate, which is why relays can safely isolate circuits._**

### 1.2 Types of Relays

- **Electromechanical Relay (EMR):** Uses moving parts and a coil.
- **Solid State Relay (SSR):** No moving parts, uses semiconductors.
- **Reed Relay:** Very small, uses magnetic reeds.

**_If you’re just starting out, EMRs are the ones you’ll most often encounter._**



## 2. Features

* **Coil Voltage:** 3V–48V DC or AC. **_(This is the voltage you supply to activate the relay.)_**
* **Contact Ratings:** up to tens of amps. **_(How much current the switched device can draw.)_**
* **Isolation** between control and load circuits. **_(Prevents the high-power side from damaging your low-power microcontroller.)_**
* **Switching Types:** NO (Normally Open), NC (Normally Closed), Changeover.  
  **_(NO = off until activated; NC = on until activated.)_**



## 4. How to Use
### Safety Note
Avoid exceeding contact voltage/current; arcing can damage contacts.  
**_Arc = tiny spark that jumps when the switch opens/closes. This can wear out the relay or be dangerous at high voltage._**



### 4.1 Identify pins

* **Coil pins:** Connect to control voltage (from Arduino or via transistor).  
* **Common (COM):** The moving part of the switch.  
* **Normally Open (NO):** COM connects here only when relay is activated.  
* **Normally Closed (NC):** COM connects here when relay is not activated.

<img src="\images\Single-Channel-Relay-Module-Pinout.jpg" width="500" height="300" alt="Relay pinout">

**_Tip: On modules, these pins are often labeled right on the board, so double-check before wiring._**



### 4.2 Driving a relay

* Use transistor or MOSFET to drive coil from microcontroller. **_(Most microcontrollers can’t power a relay coil directly, the transistor acts as a helper switch.)_**
* Add a **flyback diode** across coil to prevent damage.  
  **_(This diode stops voltage spikes created when the coil turns off from damaging your electronics.)_**



### 4.3 Applications

* Switching high-power loads (lamps, motors, heaters).  
* Isolation between circuits.  
* Automotive control (horns, lights, pumps).

**_Common beginner project: Turn on a desk lamp using Arduino + relay when a sensor triggers._**



## Video Explanation
video coming soon