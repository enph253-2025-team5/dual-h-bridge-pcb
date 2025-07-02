# Dual H-Bridge PCB

Dual h-bridge design with a PWM signal and direction bit for controlling two motors.

Similar to Greg Reid's 2025 h-bridge design, without relying on tripping the overcurrent protection. Instead, this design duplicates the incoming PWM signal, sends one to each of the low side h-bridge MOSFETs, then pulls the gate with the enhanced high side MOSFET low (avoiding shoot-through). 

Based on many factors (motor inertia, gate driver response, optocoupler distortion) the PWM frequency should be limited on the order of 100 Hz.
Intended motor battery configuration of 4S.

**BOM, Schematic, and PCB drawings in the latest release.**

## Images
![dual-h-bridge-front](https://github.com/user-attachments/assets/4387c79c-de4c-459d-a0df-f1b6483a3be2)
![dual-h-bridge-back](https://github.com/user-attachments/assets/b2b01dc3-2eff-4b83-968c-584158163c69)
![dual-h-bridge-orthographic](https://github.com/user-attachments/assets/eb019c8d-8faa-4a5a-b2cc-70eb42476243)

Designed by George Sleen.
