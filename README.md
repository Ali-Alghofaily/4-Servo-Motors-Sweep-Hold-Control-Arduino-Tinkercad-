# 4-Servo-Motors-Sweep-Hold-Control-Arduino-Tinkercad-
this Circuit is for my summer training task at Smart Methods

# 4 Servo Motors Sweep & Hold Control (Arduino Tinkercad)

This project demonstrates the control of 4 Micro Servo Motors using an Arduino Uno simulated on **Autodesk Tinkercad**.

## 🎯 Task Requirements
1. Run all 4 servo motors in a continuous **Sweep motion** (back and forth) for **2 seconds**.
2. Immediately hold all motors locked at a **90-degree angle** after the 2-second duration expires.

---

## 🔌 Pin Configuration

| Component | Pin / Connection |
| :--- | :--- |
| **Servo 1 Signal** | Digital Pin 8 |
| **Servo 2 Signal** | Digital Pin 9 |
| **Servo 3 Signal** | Digital Pin 10 |
| **Servo 4 Signal** | Digital Pin 11 |
| **VCC (All Servos)** | Arduino 5V |
| **GND (All Servos)** | Arduino GND |

---

## 🛠️ Implementation Strategy

* The `millis()` function tracks the exact execution time without blocking execution indefinitely.
* The loop logic executes inside `setup()` so that the motion sequence runs **once** when powered on, keeping the `loop()` empty to maintain the static 90-degree position indefinitely.
