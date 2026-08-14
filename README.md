# Spider-Bot 

A 4-legged robotics project built upon the open-source [Sesame Robot](https://github.com/dorianborian/sesame-robot) framework. This project uses the original ESP32-powered quadruped as a functional spider-bot.

## Features
* **Quadruped Design:** 3D-printed chassis and leg linkages (`L1`–`L4`, `R1`–`R4`) using the original movement system for 4 independent legs.
* **ESP32 Core:** Powered by the ESP32 microcontroller with a built-in captive portal for Web UI control.
* **Emotive OLED Display:** Features a 128x64 OLED screen acting as a reactive face that syncs with movement. 
* **JSON API:** Fully controllable programmatically via Python, JavaScript, and more.
* **Custom Animations:** Uses Sesame Studio to visually design stop-motion-style movements and automatically generate the necessary C++ code.

## Hardware & Build
* **Microcontroller:** ESP32 (DevKitC or S2 Mini).
* **Actuators:** MG90S metal-gear servos.
* **Display:** 128x64 I2C OLED.
* **3D Printed Parts:** Designed for PLA with minimal supports.

## Acknowledgments
Based on the [Sesame Robot](https://github.com/dorianborian/sesame-robot) created by Dorian Todd.
