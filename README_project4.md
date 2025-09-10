# EE 533 – Neuromorphic Computing — Project 4

**Course:** EE 533 — Neuromorphic Computing  
**Term:** Spring 2025  
**Due Date:** April 28, 2025  
**Institution:** San Diego State University  

---

## 📌 Project Description

In this project, you will design a **toy spiking neural network (SNN)** with two pre-synaptic input neurons (**N1** and **N2**) and one output neuron (**Nout**).  
The output neuron should be implemented as a **Leaky Integrate-and-Fire (LIF) neuron**, while the input neurons will use **square current sources**.  

Simulation and validation will be performed in **Cadence Virtuoso**:contentReference[oaicite:1]{index=1}.  

---

## 🧪 Task

- Set up an SNN with:  
  - **Two input neurons (N1, N2):** driven by square current sources (`ipulse` from `NCSU_Analog_Parts/Current_Sources`) with **100 μs pulse width**.  
  - **One output neuron (Nout):** LIF neuron with leakage included.  
- Add a leakage MOSFET (**Mleak**) in parallel with the membrane capacitor.  
- Use the given device parameters and dimensions in your design.  

---

## 📐 Circuit Parameters

- **Membrane Capacitor:** Cmem = 4 pF  
- **Feedback Capacitor:** CFB = 1 pF  
- **CMOS Inverters:**  
  - Wp/Lp = 10 μm / 2 μm  
  - Wn/Ln = 4 μm / 2 μm  
- **pMOS Current Mirrors (N1, N2 injection currents):** W/L = 10 μm / 10 μm  
- **M1, M2:** W/L = 4 μm / 2 μm  
  - M2 gate controlled by **Vb** to set output pulse width (~100 μs)  
- **Mleak:** W/L = 4 μm / 2 μm, gate controlled by **Vleak = 250 mV**  

---

## ⚙️ Specifications

Adjust the weights **w1** and **w2** so that **Nout** fires under these conditions:  

- Every **third firing event** of **N1** (firing at 200 Hz) when **N2 is silent**.  
- Every **fifth firing event** of **N2** (firing at 200 Hz) when **N1 is silent**.  

---

## 📑 Report Requirements

Your report must include:  

1. Hand calculations to determine **w1 and w2**, using simulated values for **Vmem,reset**, **Vmem,threshold**, and the leakage current of the output neuron.  
2. Screenshot of the **schematics**.  
3. Verification that the specifications are satisfied by showing:  
   - Input current waveforms (N1, N2).  
   - Output neuron voltage waveform (Nout).  
4. If unable to meet the specs, provide a short explanation of possible issues. Otherwise, omit discussion.  

---
