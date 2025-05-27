# CAN-Bus-Communication-System-for-Smart-Diagnostics-in-Autonomous-Vehicles-using-the-STM-32
This project presents a **low-cost, fault-tolerant Controller Area Network (CAN) Bus communication system** designed for **autonomous vehicle diagnostics**. It enables efficient and reliable data exchange between Electronic Control Units (ECUs), helping to enhance performance and safety in real-time autonomous operations.
# 🚗 Low-Cost ECU-Based CAN Bus Communication System for Smart Diagnostics in Autonomous Vehicles

## 📘 Overview  
![image](https://github.com/user-attachments/assets/15c490f4-b829-498e-8b10-70f1e745aa19)

This project presents a **low-cost, fault-tolerant Controller Area Network (CAN) Bus communication system** designed for **autonomous vehicle diagnostics**. It enables efficient and reliable data exchange between Electronic Control Units (ECUs), helping to enhance performance and safety in real-time autonomous operations.
![image](https://github.com/user-attachments/assets/c6516f4a-4e14-4542-acf9-6f07d01d972c)

---![image](https://github.com/user-attachments/assets/799ccf01-ee24-46f4-b289-be13b759cdfb)


## 🎯 Objectives
![image](https://github.com/user-attachments/assets/53af251e-ad9f-42c3-b8ac-b8a054e652af)

- Enable robust real-time communication between distributed **low-cost ECUs**
- Support high-speed, low-latency CAN Bus communication for autonomous vehicles
- Implement **fault tolerance**, **error recovery**, and **message prioritization**
- Demonstrate reduced wiring complexity and enhanced system scalability
![image](https://github.com/user-attachments/assets/0d743da2-09d1-4259-8127-575f972f2aa5)

---

## 🧠 Features

✅ Real-time data transmission over CAN  
✅ Reduced complexity with centralized communication lines  
✅ Fault tolerance and error handling  
✅ Message prioritization for safety-critical systems  
✅ Scalable architecture for multi-node autonomous platforms  
✅ Reduced cost using basic microcontrollers and standard CAN ICs

---
![image](https://github.com/user-attachments/assets/18a5c81d-80a2-4d9a-bf80-26cc9149e227)

## 🧰 Hardware Used

| Component                         | Quantity |
|----------------------------------|----------|
| Low-Cost ECUs (AVR/ARM/8051 etc.)| 2+       |
| MCP2551 CAN Transceivers         | 2+       |
| CAN Termination Resistors (120Ω) | 2        |
| Breadboards & Jumper Wires       | -        |
| 5V Power Supply or Battery       | 1        |
![image](https://github.com/user-attachments/assets/672db6c4-ef88-4684-8d7d-514fabc87da8)

---

## 🖥️ Software Used

- **Arduino IDE / Keil / MPLAB** – Firmware programming
- **Proteus / Multisim** – Simulation & circuit testing
- **CAN Libraries** – For protocol-level implementation

---

## 📊 Communication Architecture
![image](https://github.com/user-attachments/assets/f0cc54c2-d521-41e8-ac52-d0ce92497c24)
            [STM32 Master Node] ---\
                                   >==[ CAN Bus ]==> [STM32 Slave Node]
            [STM32 Slave Node] ---/

## 🧪 Experimental Setup
![image](https://github.com/user-attachments/assets/3e1aab4f-96d5-4c77-9dff-587dcacf5b54)
![image](https://github.com/user-attachments/assets/1067bd3f-a49f-4acf-b905-ee2085e7a906)

- Real-time data transmission between two or more STM32 boards.
- Testing under low and high bus load conditions.
- Fault injection to test error detection and bus-off recovery.
- Latency and integrity analysis with timestamp monitoring.

## 📊 Results

- Achieved **low-latency transmission** and high bus stability.
- **Fault recovery mechanisms** like CRC and retransmissions functioned as expected.
- CAN Bus setup demonstrated **scalability** and **robustness** for real-time autonomous applications.

## 🔍 Diagrams & Flowcharts
![image](https://github.com/user-attachments/assets/78a55116-9ef3-4af3-acd8-d521280bbf63)
![image](https://github.com/user-attachments/assets/1bda9f28-ec59-4155-bfd3-6a208f24316b)

> See `docs/` folder for:
- CAN Bus Topology Diagram
- Circuit Diagram using MCP2551
- Internal ECU Architecture
- Communication Flowchart

## ⚡ Getting Started
![image](https://github.com/user-attachments/assets/38caab6c-f4a3-42b0-ab80-e730d988c21d)

### Hardware Requirements
- STM32 Nucleo-F446 boards (or similar)
- MCP2551 CAN transceivers
- 120Ω termination resistors
- Breadboards and jumper wires
- USB-UART cable (optional for serial debug)
![image](https://github.com/user-attachments/assets/2381cadb-7447-48ed-888d-cf02a58db75a)

### Software Setup
1. Install [STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html)
2. Clone the repo and open the `.ioc` file
3. Flash firmware to each STM32 using ST-Link
4. Connect boards via MCP2551 and CAN_H/L lines




