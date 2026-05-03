# Xiao-ESP32-C3-RC-Car-Controller-PCB
A complete, circular PCB designed for an ESP32-C3-powered RC car. Features an onboard LM2577 voltage booster (1S Li-ion to VS), DRV8833 dual motor driver, Hall sensor input, and power switching. Built for compact, high-performance robotics and custom RC car projects.
# Xiao ESP32-C3 RC Car Controller PCB

![EasyEDA](https://img.shields.io/badge/Designed_in-EasyEDA-blue)
![License](https://img.shields.io/badge/License-MIT-green)

This repository contains the complete hardware design files for a **circular RC car controller PCB**. The board is designed to be embedded directly into the chassis or wheel hub of a custom RC car, utilizing the compact **Seeed Studio XIAO ESP32-C3** module for wireless (Wi-Fi/BLE) control.

![3D Render](images/3d_render.png) <!-- Remember to place your 3D render image in an 'images/' folder -->

## ✨ Key Features
-----------------------------------------------
<img width="1169" height="1001" alt="Schematic_Xiao_ESP_based_RC_Car_2026-05-02" src="https://github.com/user-attachments/assets/94297d6d-b1e3-4435-88b2-08ffe872ffcf" />

-----------------------------------------------
<img width="587" height="561" alt="Xiao_ESP_based_RC_Car_3D_Top_View" src="https://github.com/user-attachments/assets/d71a2253-585a-4a7b-bee5-0bcba63fa693" />

-----------------------------------------------
<img width="561" height="567" alt="Xiao_ESP_based_RC_Car_3D_Bottom_View" src="https://github.com/user-attachments/assets/81938319-2783-4b14-81f3-30039ef4431c" />

-----------------------------------------------
<img width="612" height="632" alt="Xiao_ESP_based_RC_Car_2D_View" src="https://github.com/user-attachments/assets/244e99e4-b9ae-4ce6-8828-c89ab9b4f551" />

-----------------------------------------------
*   **Core Processor:** **XIAO ESP32-C3** footprint (LoRa / BLE / Wi-Fi ready).
*   **Motor Control:** **DRV8833PWP** Dual H-Bridge motor driver for driving two DC motors.
*   **Power Management (Boost Converter):** **LM2577T-ADJ** boost converter steps up a single Li-ion battery (3.7V VBATT) to a higher voltage (VS) suitable for motors and other peripherals.
*   **Battery Protection Circuit:** Integrated MOSFETs (`AO3400A`, `DMP1045U-7`) and power selection circuitry for safe battery operation.
*   **Sensors & Feedback:** **JST connector (CN5)** for Hall sensors, enabling precise motor speed/direction feedback.
*   **Solenoid/Actuator Output:** An additional high-current output (`CN4`) for controlling a solenoid or other actuators.
*   **User Interface:** 3x indicator LEDs (Red, Green, Yellow) for status and debugging.

## 📂 Repository Structure
```text
/
├── images/                               # PCB renders (3D, 2D traces)
├── Schematic_Xiao_ESP_based_RC_Car_2026-05-02.pdf # Full circuit schematic
├── PCB_PCB_Xiao_ESP_based_RC_Car_2026-05-02.pdf   # PCB layout visual
├── BOM_Xiao_ESP_based_RC_Car_2026-05-02.csv       # Bill of Materials
└── PickAndPlace_PCB_Xiao_ESP_based_RC_Car_2026-05-02.csv # Pick & Place coordinates
