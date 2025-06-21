# Enhanced RPM Monitoring System with Over-Speed Alarm

## Project Title
**Indicator of Digital RPM for Electrical Motor using Alarm Indicator with Over Speed**

## Abstract
This project implements a **Digital RPM Indicator** with an **Over-Speed Alarm** using the **8052 microcontroller**. It is designed to measure the RPM of an electric motor non-contactly using an **IR sensor** and activate a **buzzer alert** if the RPM exceeds a defined safety limit. The system displays real-time RPM values on a **16x2 LCD**.

---

## Features
- Real-time RPM monitoring
- Over-speed alert through buzzer
- LCD display for RPM and alerts
- Non-contact sensing using IR
- Embedded system using 8052 microcontroller

---

## Components Used
- 8052 Microcontroller
- IR Sensor Module
- 16x2 LCD Display
- Buzzer
- Motor with reflective blades
- Power Supply (5V regulated)

---

## Working Principle
- The **IR sensor** detects each revolution of the motor shaft.
- The microcontroller counts the number of IR pulses in 1 second.
- RPM is calculated using the formula:  
  `RPM = (Number of Interruptions per second * 60) / Number of Blades`
- If the RPM exceeds **1000**, the **buzzer** is triggered and an “OVER SPEED!” message is displayed.

---

## Circuit Connections
- **IR Sensor Output** → P1.0 (IR Input)
- **LCD Data Pins (D0-D7)** → P3
- **LCD Control Pins**:  
  - RS → P2.0  
  - RW → P2.1  
  - EN → P2.2
- **Buzzer** → P0.2

---
## Circuit diagram
Shown in the pdf attached in repository

---
## How to Run
1. Burn the code into the 8052 microcontroller using a compatible programmer.
2. Connect the components as per the circuit diagram.
3. Power the system using a 5V DC supply.
4. On power-up, the LCD displays welcome messages followed by the current RPM.
5. If RPM > 1000, buzzer turns on and warning message appears.

---

## Applications
- Industrial motor speed monitoring
- Safety systems for over-speed protection
- Educational microcontroller projects

---




