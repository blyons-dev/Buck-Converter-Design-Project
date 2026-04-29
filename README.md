# Buck Converter Design Project
This project focuses on the design and implementation of a DC-DC Buck Converter system controlled by an Arduino Nano. The system dynamically adjusts the duty cycle of a PWM signal to regulate and stabilize the output voltage under varying conditions.
## Overview
The goal of this project is to develop a reliable and flexible buck converter that demonstrates closed-loop control using a microcontroller. By leveraging the Arduino Nano, the system can monitor output voltage and automatically adjust the switching behavior to maintain a desired voltage level. The system can also optionally be controlled using an external function generator.
## Features
- Closed-loop voltage regulation using PWM control
- Arduino Nano-based control system
- Adjustable duty cycle for output voltage tuning
- Modular design for testing and iteration
- Suitable for control algorithm development and experimentation
## System Architecture
The system consists of three main components:
- Power Stage: Includes the switching element, diode, inductor, and capacitor forming the buck converter
- Control System: Arduino Nano generating PWM and adjusting duty cycle
- Feedback Network: Voltage sensing circuit used for regulation
## Schematic Diagram
<img width="1326" height="485" alt="image" src="https://github.com/user-attachments/assets/d6563cd4-98d6-40e4-b99b-45cc8a7f4188" />

## PCB Layout (Mimics layout of perfboard)
<img width="1124" height="775" alt="image" src="https://github.com/user-attachments/assets/e8221ad3-e77f-4df6-a713-5c34ee16b166" />

## Circuit Prototype


## How It Works
1. The Arduino Nano generates a PWM signal.
2. The duty cycle of the PWM signal controls the average output voltage of the buck converter.
3. The output voltage is measured through a feedback circuit.
4. The Arduino adjusts the duty cycle in real time to maintain the desired output voltage.
## Applications
- Power supply design
- Embedded control systems
- Educational demonstrations of DC-DC conversion
- Development of control algorithms for power electronics
