# 🤖 TinyML-Based Hand Gesture Control Robot

> A wireless hand gesture-controlled robot powered by **TinyML + ESP32 + MPU6050 + NRF24L01**, enabling real-time robot movement using natural hand motions without traditional remotes.

## 📌 Project Overview

This project uses **Tiny Machine Learning (TinyML)** to recognize hand gestures on an ESP32 microcontroller and wirelessly control a robot car.  
Instead of joysticks or remote controllers, the system interprets gestures like:

- ✋ Forward  
- ✋ Backward  
- ✋ Left  
- ✋ Right  
- ✋ Still  

The recognized gesture is transmitted via **NRF24L01** to an Arduino Nano receiver, which controls the motors through a motor driver.

---

## 🚀 Key Features

- 🧠 **On-device TinyML inference** (No cloud required)
- 📡 **Wireless communication using NRF24L01**
- 🎯 **97.8% Gesture Classification Accuracy**
- ⚡ **Low latency real-time control**
- 🔋 **Low power and cost-efficient**
- 📺 **OLED display feedback**
- 🤝 Natural Human-Robot Interaction

---

## 🛠️ Hardware Components

### Transmitter Side:
- ESP32
- MPU6050 (Accelerometer + Gyroscope)
- NRF24L01
- OLED Display
- Battery Supply

### Receiver Side:
- Arduino Nano
- NRF24L01
- DRV8833 Motor Driver
- N20 BO Motors
- Robot Chassis
- 9V Battery + Voltage Regulator

---

## 🧩 System Architecture

```text
Hand Gesture
     ↓
 MPU6050 Sensor
     ↓
    ESP32
(TinyML Model)
     ↓
 NRF24L01 Transmitter
     ↓
 NRF24L01 Receiver
     ↓
 Arduino Nano
     ↓
 DRV8833 Driver
     ↓
 Robot Movement
