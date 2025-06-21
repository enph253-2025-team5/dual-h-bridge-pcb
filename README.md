# Dual H-Bridge PCB

Dual h-bridge design with a PWM signal and direction bit for controlling two motors.

Similar to Greg Reid's 2025 h-bridge design, however this design doesn't rely on tripping the overcurrent protection  then recharging the timing capacitor. Instead, this design duplicates the incoming PWM signal on each low side h-bridge MOSFET gate, and forces the gate low on the same with the high side h-bridge MOSFET enhanced (avoiding shoot-through). 

Based on many factors (motor inertia, gate driver response, optocoupler distortion) the PWM frequency should be limited on the order of 100 Hz.
Intended motor battery configuration of 4S.

### Schematic
[dual-h-bridge-schematic.pdf](https://github.com/user-attachments/files/20844989/dual-h-bridge.pdf)

### Images
![dual-h-bridge-front](https://github.com/user-attachments/assets/3388f787-9b92-459c-8d73-0a7ebf54b359)
![dual-h-bridge-back](https://github.com/user-attachments/assets/51493b0d-188c-4588-925b-199167422795)

![dual-h-bridge-orthographic](https://github.com/user-attachments/assets/326b64f2-1bd2-43ca-92aa-49003e03fca4)

Designed by George Sleen.
