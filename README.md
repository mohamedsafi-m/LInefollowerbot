# Line Follower Robot using Raspberry Pi Pico

## Overview
This project implements a simple **line follower robot** using the **Raspberry Pi Pico**, IR sensors, and a motor driver.  
The robot detects a black line on a surface and adjusts its movement to follow the path automatically.

## Components Used
- Raspberry Pi Pico
- IR Sensor Modules (2)
- Motor Driver Module
- DC Motors
- LM7805 Voltage Regulator
- Battery
- Capacitors and Resistors

## Power Supply
A **LM7805 voltage regulator** is used to provide a stable **5V supply** from the battery to the motor driver and control circuitry.

## Connections
### IR Sensors
- GP14 → Left IR Sensor Output  
- GP15 → Right IR Sensor Output  
- 3V3 → Sensor VCC  
- GND → Sensor GND  

### Motor Driver
- GP16 → IN1  
- GP17 → IN2  
- GP18 → IN3  
- GP19 → IN4  
- GND → Common Ground  

### Motors
- OUT1 & OUT2 → Left Motor  
- OUT3 & OUT4 → Right Motor  

## Working Principle
The IR sensors detect the contrast between the **black line and the background surface**.  
Based on sensor outputs, the Raspberry Pi Pico controls the motor driver to move the robot **forward, left, or right** to stay on the line.

## Tools Used
- Altium Designer (schematic design)
- Raspberry Pi Pico
- Embedded programming (MicroPython/C)
