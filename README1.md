# EE 533 – Neuromorphic Computing — Project 2

**Course:** EE 533 — Neuromorphic Computing  
**Term:** Spring 2025  
**Due Date:** March 14, 2025  
**Institution:** San Diego State University  

---

## 📌 Project Description

In this project, you will design a **signal processing circuit** capable of computing the **square of an input current (Iin)**.  
The design must be implemented in **TSMC 350nm CMOS technology** and validated through schematic simulations in **Cadence Virtuoso**:contentReference[oaicite:0]{index=0}.  

You may use multiple independent sources (voltage or current) as needed for input current setting, supply voltages, and biasing.  

---

## 🧪 Task

- **Design and simulate a current-squaring circuit.**

---

## 📐 Specifications

- Input current range: **1 nA – 10 nA**  
- Device sizing: **W/L = 20 µm / 10 µm**  
- Supply voltage: **VDD = 3.2 V**  

---

## ⚙️ Approach

### 1. Design Setup
- Set all MOS device sizes to **W/L = 20 µm / 10 µm**.  
- Use a single-supply **VDD = 3.2 V**.  

### 2. V0 Selection
a. Perform a **.DC analysis** to simulate **VDS vs V0** for V0 sweeping from 0 → 3.2 V.  
b. Using **MATLAB** (or Cadence ADE Calculator), identify a **V0 range** where **all devices** (in the translinear loop, current sinks, and current sources) operate in the **weak-inversion saturation region**.  
c. If no suitable V0 range is found, adjust the **(W/L)** accordingly.  

### 3. Circuit Validation
a. Once V0 is set, perform a **.DC analysis** to observe how **Iout varies with Iin**.  
b. Compute the **Mean Absolute Percentage Error (MAPE)** between the **true values** and the **simulated values**.  

---

## 📑 Report Requirements

Your report must include:  
1. Screenshot of the **circuit schematic**.  
2. Explanation of how **V0** was determined.  
3. Confirmation that all devices are operating in **weak-inversion saturation**.  
4. **Iout vs Iin plots** for both simulated and true values.  
5. Computation of **MAPE**, and a brief **discussion** on agreement and discrepancies.  

---
