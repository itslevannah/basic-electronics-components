---
title: Arduino Uno
layout: home
parent: Microcontrollers & Communication Modules
nav_order: 59
---

# Arduino Uno

## 1. Definition
The **Arduino Uno** is one of the most popular microcontroller boards for beginners and hobbyists.  
It’s based on the **ATmega328P microcontroller** and is designed to be easy to use for building electronic projects.

<img src="\images\Arduino_Uno_-_R3.jpg" width="500" height="300" alt="Arduino Uno Board">

## 2. Features
- **14 Digital I/O Pins** (6 can be used as PWM outputs).  
- **6 Analog Input Pins** for reading sensors.  
- **USB Connection** for uploading code and communication with a computer.  
- **Power Jack** to connect external power supply (7–12V recommended).  
- **Clock Speed**: 16 MHz.  
- **Onboard Reset Button** to restart the program.  

## 3. How It Works
1. You connect the Arduino Uno to your computer with a USB cable.  
2. Write code in the **Arduino IDE** (or other supported editors).  
3. Upload the code to the board.  
4. The microcontroller runs your program and controls connected sensors, LEDs, motors, etc.  

## 4. Common Uses
- Controlling LEDs and buzzers.  
- Reading data from sensors (temperature, light, motion, etc.).  
- Running small robots or cars.  
- Displaying information on LCDs or OLEDs.  
- Home automation projects.  

## 5. Example
A simple example to blink the onboard LED:

```cpp
void setup() {
  pinMode(13, OUTPUT);   // Set digital pin 13 as output
}

void loop() {
  digitalWrite(13, HIGH); // Turn LED on
  delay(1000);            // Wait 1 second
  digitalWrite(13, LOW);  // Turn LED off
  delay(1000);            // Wait 1 second
}
```

## 6. Video Explanation
Video coming soon