# 🗑️ Smart Contactless Dustbin using STM32 & Ultrasonic Sensor

## 📌 Overview

This project implements a **smart contactless dustbin** that automatically opens and closes its lid when a user’s hand is detected nearby. It uses an ultrasonic sensor to measure distance and a servo motor for lid actuation.

The system improves **hygiene**, reduces physical contact, and demonstrates real-world embedded system design using an STM32 microcontroller.

---

## 🎯 Features

* 🚫 Contactless operation (touch-free)
* 📏 Distance-based detection (up to 30 cm)
* ⚙️ Servo-controlled lid mechanism
* 🔄 Automatic open and close functionality
* 💡 Low-cost and easy to build

---

## 🧠 Working Principle

1. The ultrasonic sensor continuously measures the distance.
2. When an object (hand) is detected within a predefined range (≤ 30 cm),
   → the servo motor rotates to open the lid.
3. After a delay (or when the object is removed),
   → the lid automatically closes.

---

## 🧰 Components Required

* STM32 Nucleo Board (STM32C031C6)
* Ultrasonic Sensor (HC-SR04)
* Servo Motor (SG90)
* Breadboard
* Jumper Wires
* External 5V Power Supply

---

## 🔌 Circuit Connections

### Ultrasonic Sensor:

* VCC → 5V
* GND → GND
* TRIG → PA0
* ECHO → PA1 (via voltage divider)

### Servo Motor:

* VCC → External 5V
* GND → GND (common ground)
* Signal → PA6 (PWM)

⚠️ Note: Use a voltage divider for ECHO pin (5V → 3.3V) to protect the STM32.

---

## 💻 Software & Tools

* STM32CubeIDE (for firmware development)
* Wokwi Simulator (for initial testing)
* Embedded C (HAL drivers)

---

## 🧪 Simulation

The project was first tested using Wokwi simulation with an STM32 (Blue Pill equivalent), and later adapted for STM32C031C6 hardware.

---

## 🚀 How to Run

### In Simulation (Wokwi):

1. Create STM32 project
2. Connect servo and ultrasonic sensor
3. Upload Arduino-based simulation code
4. Adjust distance and observe servo movement

### On Hardware:

1. Configure pins and timers in STM32CubeIDE
2. Generate code using CubeMX
3. Flash code using ST-Link
4. Power the system and test with hand detection

---

## 📸 Results

* Lid opens automatically when hand is detected within 30 cm
* Closes after a short delay
* Smooth and responsive operation

---

## 🔧 Future Improvements

* OLED display for status indication
* Fill-level detection system
* Bluetooth / mobile app control
* Battery-powered portable design
* Buzzer or LED indication

---

## 🏆 Applications

* Smart homes
* Hospitals and clinics
* Public sanitation systems
* Offices and kitchens

---

## 📚 Learning Outcomes

* STM32 GPIO and timer configuration
* PWM signal generation
* Sensor interfacing (Ultrasonic)
* Embedded system design workflow
* Simulation to hardware implementation

---

## 👨‍💻 Author

Your Name
V.Venkata Harinath 
ECE Diploma 
SVGP TIRUPATI.
---

## 📄 License

This project is open-source and available under the MIT License.
