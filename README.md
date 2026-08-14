# Spider-Bot 

A 4-legged robotics project built upon the open-source [Sesame Robot](https://github.com/dorianborian/sesame-robot) framework. This project uses the original ESP32-powered quadruped as a functional spider-bot.

## Features
* **Quadruped Design:** 3D-printed chassis and leg linkages (`L1`–`L4`, `R1`–`R4`) using the original movement system for 4 independent legs.
* **ESP32 Core:** Powered by the ESP32 microcontroller with a built-in captive portal for Web UI control.
* **Emotive OLED Display:** Features a 128x64 OLED screen acting as a reactive face that syncs with movement. 
* **JSON API:** Fully controllable programmatically via Python, JavaScript, and more.
* **Custom Animations:** Uses Sesame Studio to visually design stop-motion-style movements and automatically generate the necessary C++ code.

## 3D Printing
* **Material:** PLA / PLA+
* **Infill:** 8-10%
* **Wall Loops:** 2
* **Infill Pattern:** Honeycomb

| Top Cover | Support Required |

### Top Cover Settings (Original Style)

Brim: Outer brim only
Support type: Normal (Manual)

## Hardware & Build
* **Microcontroller:** ESP32 (DevKitC or S2 Mini).
* **Actuators:** MG90S metal-gear servos.
* **Display:** 128x64 I2C OLED.
* **3D Printed Parts:** Designed for PLA with minimal supports.

## Core Electronics

| Item | Qty | Notes | Source |
| --- | --- | --- | --- |
| MG90S all-metal micro servos (180 Deg) | 8 (buy 10 for spares) | Primary hip/leg actuators; includes servo horns but keep extras | [Amazon](https://www.amazon.com/s?k=mg90s+metal+gear+servo+pack+of+8) |
| 0.96" SSD1306 I2C OLED | 1 | 128x64 display that slides into the top cover slot | [Amazon](https://www.amazon.com/s?k=0.96%22+I2C+OLED+SSD1306) |
| USB-C data/power cable | 1 | Needs to carry 5V/3A for flashing and tethered mode | [Amazon](https://www.amazon.com/s?k=usb+c+cable+60w) |
| Rocker power switch (KCD1, panel mount) | 1 | Snaps into the top cover cutout | [Amazon](https://www.amazon.com/s?k=KCD1+mini+rocker+switch+2+pin) |
| 22AWG silicone wire kit | 1 | Power/ground bus lines | [Amazon](https://www.amazon.com/s?k=22awg+silicone+wire+kit) |
| 30AWG silicone wire kit | 1 | Signal leads and dense harnessing | [Amazon](https://www.amazon.com/s?k=30awg+silicone+wire) |
| Heat-shrink assortment | 1 | Insulate OLED, switch, and battery joints | [Amazon](https://www.amazon.com/s?k=heat+shrink+tubing+kit) |
| Small zip ties | 1 pack | Bundling wires inside the frame | [Amazon](https://www.amazon.com/s?k=mini+zip+ties) |

| Item | Qty | Notes | Source |
| --- | --- | --- | --- |
| Lolin/WeMos ESP32-S2 Mini | 1 | Native USB-C, fits on perfboard for the hand-wired build | [Amazon](https://www.amazon.com/s?k=esp32+s2+mini) |
| Small protoboard (approx. 5×7 cm) | 1 | Hosts the header matrix and rails | [Amazon](https://www.amazon.com/s?k=prototype+perfboard) |
| 3-pin male headers | 8 | Build the servo breakout; match spacing to MG90 plugs | [Amazon](https://www.amazon.com/s?k=pin+header+strip) |
| Buck converter (5–12 V in to stable 5V/3A out) | 1 | Powers motors + MCU when using batteries | [Amazon] (https://www.amazon.com/sk=3a+dc+dc+buck+converter+module) |

## Acknowledgments
Based on the [Sesame Robot](https://github.com/dorianborian/sesame-robot) created by Dorian Todd.
