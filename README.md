# 🔥 Fire Control System using Arduino
## 📖 Overview
This project is a Fire Detection and Warning System using an NTC Thermistor, an LCD display, a buzzer, and a red LED, all powered by an Arduino Nano. It continuously monitors temperature changes and triggers visual and audible alerts if fire conditions are detected.

## 🧰 Components Used
### Arduino Nano

### NTC Thermistor (Temperature Sensor)

### 16x2 LCD Display

### Red LED

### Buzzer

### Potentiometer (for LCD contrast)

### Breadboard & Jumper wires

### Resistors

## ⚙️ How it Works
### 🔸 Normal Operation:
#### The system continuously reads the ambient temperature.

#### Real-time temperature is displayed on the LCD.

### ⚠️ Warning Mode:
#### Condition: Temperature exceeds the warning threshold.

#### Action:

LCD shows Warning: FIRE!

Buzzer emits warning beeps.

### 🚨 Critical Mode:
#### Condition: Temperature exceeds the danger threshold.

#### Action:

LCD displays Run away now!!

Buzzer tone becomes more urgent.

Red LED turns on to indicate danger.

## 🛠️ Circuit Overview

The thermistor is part of a voltage divider connected to an analog pin. The system uses a simple logic in the Arduino sketch to classify the temperature and take action accordingly.

## 📋 Applications
### Fire detection in homes or labs

### Educational demonstrations of sensor-based systems

### Safety monitoring for temperature-sensitive environments

## 🧪 Example Thresholds (Configurable)
### Mode	          ||   Temperature (°C)       ||     	System Response
### Normal	        ||      < 45°C	            ||      Display temperature only
### Warning      	  ||     45–65°C	            ||      LCD warning + buzzer
### Critical Alert	||      > 65°C	            ||      LCD alert + loud buzzer + red LED

