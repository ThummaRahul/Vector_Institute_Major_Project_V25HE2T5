# 🚗 MULTI-ECU VEHICLE MONITORING USING CAN

## 📌 Project Overview

**MULTI-ECU Vehicle Monitoring Using CAN** is a B.Tech major embedded systems project that demonstrates real-time vehicle parameter monitoring using multiple Electronic Control Units (ECUs) communicating over the **Controller Area Network (CAN)** protocol. The system acquires, processes, and displays data such as **engine temperature**, **battery status**, and **indicator states** on an embedded LCD.

This project closely resembles real-world **automotive embedded systems** used in modern vehicles.

---

## 🎯 Aim

To design and develop a multi-ECU vehicle monitoring system using the Controller Area Network (CAN) protocol that acquires, decodes, and displays real-time data from multiple ECUs, enabling effective monitoring of key vehicle parameters such as battery status, engine temperature, and system warning indicators through a user-friendly embedded display.

---

## 🧠 Project Insight

* Knowledge of **Embedded C programming**
* Thorough understanding of **LPC2129 architecture**
* Hands-on experience with **GPIO, ADC, Interrupts, CAN interface**
* Practical implementation of **CAN protocol in automotive systems**

---

## 🧩 System Architecture

The system consists of **three independent ECUs (nodes)** connected through a CAN bus:



### 🔹 Main Node

* Reads engine temperature using **DS18B20**
* Displays parameters on **LCD**
* Sends indicator control commands to Indicator Node
* Receives battery status from Battery Node via CAN

### 🔹 Indicator Node

* Listens to CAN messages from Main Node
* Controls **8 LEDs** to represent vehicle indicators
* Implements left-to-right and right-to-left scrolling LED pattern

### 🔹 Battery Node

* Monitors battery level using **ADC (Potentiometer)**
* Simulates battery percentage (0–100%)
* Sends battery status to Main Node via CAN

---

## 🖼️ Block Diagram

![image alt](https://github.com/ThummaRahul/Vector_Institute_Major_Project_V25HE2T5/blob/main/Delay_Files/Screenshot%202026-01-26%20155927.png?raw=true)

## 🔧 Hardware Requirements

* LPC2129 Microcontroller
* CAN Transceiver (MCP2551)
* LCD (20x4)
* LEDs (8)
* Push Buttons / Switches
* Potentiometer (Battery Simulation)
* DS18B20 Temperature Sensor

![image alt](https://github.com/ThummaRahul/Vector_Institute_Major_Project_V25HE2T5/blob/main/Delay_Files/InShot_20260210_202554761.jpg.jpeg?raw=true).

---

## 💻 Software Requirements

* Embedded C Programming
* Keil µVision (C Compiler)
* Flash Magic (Programming Tool)

---

## 🛠️ Implementation Sequence

1. Create a project folder and organize files by node
2. Test LCD interface (characters, strings, integers)
3. Interface active-low switches and display status on LCD
4. Interface DS18B20 temperature sensor and display engine temperature
5. Test ADC using potentiometer and display voltage value
6. Verify external interrupts (EINT0 & EINT1)
7. Test basic CAN communication using reference code
8. Develop individual node logic
9. Integrate all nodes over CAN bus
10. Verify real-time data exchange and LCD output

---

![image alt](https://github.com/ThummaRahul/Vector_Institute_Major_Project_V25HE2T5/blob/main/Delay_Files/Screenshot%20(94).png?raw=true).

---

## 📁 Project Folder Structure

```
Multi-ECU-Vehicle-Monitoring-Using-CAN/
│
├── Main_Node/
│   ├── main.c
│   ├── can.c
│   ├── lcd.c
│   └── ds18b20.c
│
├── Indicator_Node/
│   ├── indicator.c
│   └── can.c
│
├── Battery_Node/
│   ├── battery.c
│   └── adc.c
│
├── Docs/
│   ├── block_diagram.png
│   └── project_report.pdf
│
├── README.md

---

## 🚀 Applications

* Automotive embedded systems
* Vehicle diagnostics
* ECU communication systems
* CAN-based industrial automation

---

## 🔮 Future Enhancements

* Replace potentiometer with real battery monitoring circuit
* Add CAN error detection and logging
* Integrate GSM/GPS for remote vehicle monitoring
* Upgrade display to graphical LCD or TFT

---

## 👨‍💻 Presented By ->

**T. Rahul**

B.Tech – Electrical and Electronics Engineering

---

## 🎓 Project Guide

Chandramouli Sir
(Project Guide / Tutor)

Embedded Systems | CAN | LPC2129  


