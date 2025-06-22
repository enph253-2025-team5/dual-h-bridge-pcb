# Dual H-Bridge PCB

Dual h-bridge design with a PWM signal and direction bit for controlling two motors.

Similar to Greg Reid's 2025 h-bridge design, without relying on tripping the overcurrent protection. Instead, this design duplicates the incoming PWM signal, sends one to each of the low side h-bridge MOSFETs, then pulls the gate with the enhanced high side MOSFET low (avoiding shoot-through). 

Based on many factors (motor inertia, gate driver response, optocoupler distortion) the PWM frequency should be limited on the order of 100 Hz.
Intended motor battery configuration of 4S.

**BOM, Schematic, and PCB drawings in the latest release.**

## Images
![dual-h-bridge-front](https://github.com/user-attachments/assets/3388f787-9b92-459c-8d73-0a7ebf54b359)
![dual-h-bridge-back](https://github.com/user-attachments/assets/41d2673e-8f9d-45f6-935b-dc5720f4d4b1)
![dual-h-bridge-orthographic](https://github.com/user-attachments/assets/326b64f2-1bd2-43ca-92aa-49003e03fca4)

Designed by George Sleen.
