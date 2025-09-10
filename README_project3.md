# EE 533 – Neuromorphic Computing — Project 3

**Course:** EE 533 — Neuromorphic Computing  
**Term:** Spring 2025  
**Due Date:** April 9, 2025  
**Institution:** San Diego State University  

---

## 📌 Project Description

In this project, you will design an **Integrate-and-Fire (I&F) neuron** that receives a current as input and generates a **pulse train** at its output.  
The **pulse train frequency** must be a function of the input current:contentReference[oaicite:1]{index=1}.  

---

## 🧪 Task

- Design and simulate a **simple I&F neuron circuit**.  
- Verify that the output pulse frequency varies linearly with input current.  

---

## 📐 Specifications

- Output pulse width: **~10 μs**  
- Input current range: **1 nA – 10 nA**  
- Output pulse rate (PR) must linearly vary between **10 Hz – 100 Hz**  
  - At **1 nA**, PR = 10 Hz  
  - At **2.8 nA**, PR = 28 Hz  
  - At **10 nA**, PR = 100 Hz  
- Supply voltage: **VDD = 3.2 V**  

---

## ⚙️ Notes & Design Guidance

- Review the **I&F neuron circuit** from lecture.  
- Key relations:  
  - Pulse width (**tH**) is influenced by **Cmem, Irst, and Iin**, where **Irst** is controlled by **Vpw**.  
  - Pulse rate:  
    ```
    PR = 1 / (tH + tL) ≈ 1 / tL
    ```
  - Charging relation:  
    ```
    Ctot * dVmem/dt = Iin
    ΔT = Ctot * ΔVmem / Iin
    ```
    Thus,  
    ```
    PR ≈ Iin / (Ctot * ΔVmem)
    ```  

---

## 📑 Report Requirements

Your submission must include:  

1. Hand calculations.  
2. Schematic screenshot.  
3. Table of device and capacitor sizes.  
4. 500 ms of schematic simulations showing **Iin, Vmem, and output pulses** for:  
