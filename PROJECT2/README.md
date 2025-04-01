# Transformerless AC to DC 5V Converter

This project demonstrates how to convert **220V AC to 5V DC** without using a transformer. Instead, it relies on a **capacitive dropper circuit** to reduce voltage before rectification and regulation.

---

## 📌 Table of Contents
- [Introduction](#introduction)
- [Why Transformerless Power Supply?](#why-transformerless-power-supply)
- [Circuit Diagram](#circuit-diagram)
- [Working Principle](#working-principle)
- [Components Required](#components-required)
- [PCB Design](#pcb-design)
- [Simulation](#simulation)
- [Precautions](#precautions)
- [References](#references)

---

## 🔹 Introduction
Traditional AC to DC converters use transformers to step down voltage. However, in **low-power applications**, a transformerless power supply is a cost-effective alternative. This circuit converts **220V AC** to **5V DC** safely using a capacitor, rectifier, and voltage regulator.

---

## 🔹 Why Transformerless Power Supply?
✔ **Compact Design** – No bulky transformer, making it ideal for space-limited applications.  
✔ **Cost-Effective** – Eliminates the need for expensive transformers.  
✔ **Efficient for Low Current Applications** – Suitable for circuits requiring small current (e.g., microcontrollers, small sensors).  

---

## 🔹 Circuit Diagram
📌 **[Click here to view the schematic](schematic.jpg)**  

![Transformerless AC to DC 5V Circuit](schematic.jpg)

---

## 🔹 Working Principle
1. **Voltage Dropping**  
   - **C1 (X-rated capacitor)** drops the **220V AC** voltage while limiting current.  
   - **R1 (Bleeder resistor)** discharges C1 when unplugged, preventing shock hazards.  

2. **Rectification**  
   - **Bridge Rectifier (D1 - D4)** converts AC to pulsating DC.  

3. **Smoothing**  
   - **C2 (Electrolytic capacitor)** filters the pulsating DC.  

4. **Voltage Regulation**  
   - **7805 voltage regulator** ensures a stable **5V output**.  

---

## 🔹 Components Required
| Component | Specification | Quantity |
|-----------|--------------|----------|
| X-rated Capacitor | 0.47µF, 400V | 1 |
| Resistor | 470KΩ | 1 |
| Resistor | 1KΩ | 1 |
| Diode | 1N4007 | 4 |
| Electrolytic Capacitor | 1000µF, 25V | 1 |
| Ceramic Capacitor | 0.1µF | 1 |
| Voltage Regulator | 7805 | 1 |
| LED | Indicator | 1 |

---

## 🔹 PCB Design
📌 **[Click here to view the PCB layout](pcb_layout.jpg)**  

![PCB Layout for Transformerless AC to DC 5V](pcb_layout.jpg)

---

## 🔹 Simulation
- The circuit is tested in **Proteus** and verified for stable **5V DC output**.  
- 📌 **[Click here to view simulation results](simulation_results.jpg)**  

---

## ⚠️ Precautions
❗ **High Voltage Warning:** This circuit operates at **220V AC**, which can be lethal. Always follow safety precautions:  
✔ **Do not touch the circuit when powered.**  
✔ **Use insulated gloves when testing.**  
✔ **Always discharge capacitors before handling.**  

---

## 📚 References
- Transformerless power supply design articles.  
- Datasheets for **7805, 1N4007 diodes, and X-rated capacitors**.  

---

### 📌 **Note**  
This project is suitable for **low-power applications** like microcontroller circuits, sensor modules, and LED indicators. Do **not** use it for high-current devices.  

---

