---
title: LCD (16x2)
layout: home
parent: Output Devices & Displays
nav_order: 54
---



# LCD (16x2)

## 1. Definition
### 1.1 LCD (16x2)

An LCD (Liquid Crystal Display) 16x2 module is a display device capable of showing 16 characters per line over 2 lines, commonly used in microcontroller projects for text output.

<img src="\images\51jy8enJluL._UF1000,1000_QL80_.jpg" width="500" height="300" alt="LCD 16x2 example">

**Key Features:**
- Can display letters, numbers, and symbols.
- Usually based on the HD44780 controller.
- Requires simple wiring with parallel or I2C communication.
- Low power consumption.


## 2. Types
### 2.1 Based on Backlight Color
- **Green Backlight** : Common and cost-effective.
- **Blue Backlight** : More modern, better visibility in low light.

### 2.2 Based on Interface
- **Parallel Interface** : Standard 16-pin connection.
- **I2C Interface** : Uses only 2 data pins (SDA, SCL) with an I2C adapter.


## 3. Applications
- Displaying sensor data (temperature, humidity, etc.).
- Menu navigation for embedded devices.
- Status or error messages in electronic systems.
- Time/date display in clocks.
- Interactive projects with user feedback.



## 4. Working Principle
The LCD uses liquid crystal molecules that change their orientation when an electric field is applied, controlling light passage through the display’s polarizing filters. Characters are generated using a pixel matrix for each segment.


## 5. Pin Configuration (Parallel Interface)

| Pin No. | Symbol | Description |
|---------|--------|-------------|
| 1       | VSS    | Ground |
| 2       | VDD    | +5V Power Supply |
| 3       | V0     | Contrast Adjustment |
| 4       | RS     | Register Select (0: Command, 1: Data) |
| 5       | RW     | Read/Write (0: Write, 1: Read) |
| 6       | E      | Enable Signal |
| 7-14    | D0-D7  | Data Pins |
| 15      | LED+   | Backlight Positive |
| 16      | LED-   | Backlight Negative |



## 6. Safety Notes
- Avoid direct sunlight exposure for prolonged periods, it may damage the LCD.
- Do not apply voltage beyond recommended levels.
- Handle with care; LCD glass is fragile.



## Video Explanation 
video coming soon