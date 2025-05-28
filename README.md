
# 🐾 Smart Pet Feeder (IoT-based)

This project is an IoT-based **Smart Pet Feeder** that automates feeding and monitoring of pets using an **ESP8266**, **ultrasonic sensors**, a **servo motor**, and an **LED**. It connects to **Adafruit IO** for real-time data monitoring and allows manual control through a Python-based GUI.

---

## 📦 Features

- 📡 Sends real-time data to **Adafruit IO**
- 🥣 Detects bowl food level and monitors food stock
- 🔄 Automatically closes the servo gate if the bowl is full
- 👆 Manual control of the feeder and LED via a Python GUI

---

## 🔧 Hardware Used

- ESP8266 (e.g., NodeMCU or ESP-12)
- 2x HC-SR04 Ultrasonic Sensors  
  - One to monitor the pet bowl  
  - One to monitor the food container
- SG90 Servo Motor (controls food gate)
- LED (status indication)
- Jumper wires, breadboard/PCB
- 5V regulated power supply

---

## 🧠 How It Works

- The **ESP8266**:
  - Sends bowl sensor data every 10 seconds
  - Sends stock sensor data every 30 seconds
- If the bowl distance ≤ 15 cm, the servo automatically closes the gate (0°)
- Feeder and LED can also be controlled manually using a Python GUI via **Adafruit IO**

---

## 🌐 IoT Platform

- **Adafruit IO** is used for:
  - Visualizing distance data from both sensors
  - Sending control signals to the servo and LED

---

