# 🔥 Fire Control System using Arduino

A smart **Fire Detection and Warning System** using an **NTC Thermistor**, **LCD display**, **buzzer**, and **red LED**, powered by an **Arduino Nano**. The system continuously monitors ambient temperature and provides real-time alerts when fire-like conditions are detected.

---

## 📖 Overview

This project demonstrates how to build a **sensor-based safety system** that reacts to temperature changes with **visual and audible alerts**, making it ideal for educational purposes and basic safety setups.

---

## 🧰 Components Used

- 🧠 **Arduino Nano**  
- 🌡️ **NTC Thermistor** (Temperature Sensor)  
- 🖥️ **16x2 LCD Display**  
- 🔴 **Red LED**  
- 🔊 **Buzzer**  
- 🎚️ **Potentiometer** – for adjusting LCD contrast  
- 🔌 **Breadboard & Jumper Wires**  
- 🔩 **Resistors** – for voltage divider and current limiting  

---

## ⚙️ How It Works

### 🔸 **Normal Operation**
- Continuously reads **ambient temperature**
- Displays real-time temperature on **LCD**

### ⚠️ **Warning Mode**
- **Condition**: Temperature > 45°C and ≤ 65°C  
- **Action**:
  - LCD displays: `Warning: FIRE!`  
  - Buzzer emits warning beeps  

### 🚨 **Critical Mode**
- **Condition**: Temperature > 65°C  
- **Action**:
  - LCD displays: `Run away now!!`  
  - Buzzer emits continuous urgent tone  
  - Red LED lights up to indicate danger  

---

## 🔌 Circuit Diagram

*![Simulation](https://github.com/user-attachments/assets/50d3ea03-d3ff-484d-904a-795a3e6efe70)*

---

## 🛠️ Circuit Overview

- The **NTC thermistor** is connected in a **voltage divider** configuration to an **analog pin** on the Arduino.  
- The **Arduino sketch** classifies temperature readings into **three states**:
  - Normal
  - Warning
  - Critical  
- Based on the detected state, it updates the **LCD**, triggers the **buzzer**, and turns the **LED** on/off.

---

## 📊 Example Thresholds (Customizable)

| Mode            | Temperature (°C) | System Response                            |
|-----------------|------------------|---------------------------------------------|
| Normal          | < 45°C           | Display temperature only                    |
| Warning         | 45°C – 65°C      | LCD warning + Buzzer beeps                  |
| Critical Alert  | > 65°C           | LCD alert + Continuous buzzer + Red LED ON  |

---

## 📋 Applications

- 🏠 **Home fire detection**
- 🧪 **Lab safety monitoring**
- 🎓 **Educational demonstrations**
- 🛡️ **Monitoring temperature-sensitive environments**

---

## 💻 Software

- Programmed using **Arduino IDE**  
- Code includes temperature conversion, threshold logic, and LCD/buzzer control  

---
