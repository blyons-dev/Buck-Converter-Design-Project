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
<img width="1357" height="479" alt="image" src="https://github.com/user-attachments/assets/27fc647b-5118-4e7c-9048-dc492b65f903" />

## PCB Layout
<img width="1124" height="775" alt="image" src="https://github.com/user-attachments/assets/e8221ad3-e77f-4df6-a713-5c34ee16b166" />

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
## KiCad Setup
### Installation
1. Download KiCAD from the official website.
2. Follow the installation instructions for your operating system.
3. Download and Install the Git plugin for KiCad through the Plugin and Content Manager.
### Configuration
1. Open KiCAD and open the project you'd like to use to work on the repo.
2. Initialize git in the local folder you're using and connect to GitHub.
```bash
git init
git remote add origin https://github.com/blyons-dev/BLDC-Drone.git
```
3. Switch to the current branch (replace current-branch with the branch name).
```bash
git fetch origin
git checkout -b current-branch origin/current-branch
```
4. Configure git to track the right branch.
```bash
git branch --set-upstream-to=origin/current-branch current-branch
```
4a. Optional. Verify you're on the right branch.
```bash
git branch -v
```
5. The plugin in KiCad can only be accessed in the Layout Editor, so navigate there. The plugin will automatically detect any Unstaged Changes that you have made, you just need to verify that by clicking **Rescan**.
6. Click the **Stage Changed** button to prepare everything for a commit
7. Write in the Commit Message a description of what you changed and click the **Sign Off** button as well.
8. Click **Commit** and then **Push** to send everything to the online repo.
