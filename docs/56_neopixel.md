---
title: NeoPixel / WS2812 LED Strips
layout: home
parent: Output Devices & Displays
nav_order: 56
---


# NeoPixel (Addressable RGB LEDs)

## 1. Definition
**NeoPixels** are a type of addressable RGB LED, most commonly based on the WS2812 or SK6812 chips.  
They allow control of **each LED’s color and brightness individually** using just **one data pin** from a microcontroller.  

This makes them great for creating colorful effects, animations, and displays.

<img src="\images\LED_Strip_1_1200x1200.webp" width="500" height="300" alt="NeoPixel strip example">

<img src="\images\WS2812BNon-Waterproof60Pixel_1mAddressablePixelStripROBOWAY.IN_.webp" width="500" height="300" alt="NeoPixel strip cutting">


## 2. How They Work
- Each NeoPixel has a tiny **microchip built-in** that receives data and controls the LED.
- You can chain many NeoPixels together (strips, rings, or matrices).
- Communication happens using a **special timing-based one-wire protocol**.


## 3. Applications
-  **Colorful Lighting Effects** (rainbows, fades, flashing patterns).  
-  **Music Visualizers** that react to sound.  
-  **Gaming/Arcade Projects** for interactive light displays.  
-  **Wearables and Decorations** like glowing costumes or LED art.  


## 4. Wiring
- **VCC (5V)** → Power supply.  
- **GND** → Ground.  
- **DIN** → Data input (from Arduino or other board).  
- Optional: **DOUT** → Connects to the next NeoPixel in the chain.

**Important Note**: Use a **large capacitor (1000µF, 6.3V or higher)** and a **resistor (330–470Ω)** on the data line to protect the LEDs.  



## 5. Video Explanation
Video coming soon