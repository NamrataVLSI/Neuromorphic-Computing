# Neuromorphic-Computing
MOSFET simulations in Cadence Virtuoso with MATLAB analysis: Early voltage vs channel length in strong inversion, and extraction of kappa (κ) in weak inversion
# EE 596 – Neuromorphic Computing — Project 1

**Course:** EE 596 — Neuromorphic Computing  
**Term:** Spring 2025  
**Due Date:** February 28, 2025  
**Institution:** San Diego State University  

---

## 📌 Project Description

The project involves performing MOSFET simulations using **Cadence Virtuoso** and analyzing the results in **MATLAB** and/or through hand calculations:contentReference[oaicite:0]{index=0}.  

Instructions for exporting simulation data:  
- Save a waveform from your Volta account as a `.csv` file: **Right-click → Send To → Export…**  
- Transfer the `.csv` files from Volta to your computer using **WinSCP**.  

---

## 🧪 Analysis 1: Channel-length Dependence of the Early Voltage (Strong Inversion)

1. For an **nMOS**, perform an **IDS vs VDS sweep** at **VGS = 1 V** for (W/L) = (1/1) with channel lengths:  
L = [1, 2, 5, 10, 25, 50] μm
2. Calculate the **output resistance (ro)** in the saturation region for each case.  
3. Extract the **Early voltage (VA)** using:  
ro = VA / IDS

and plot **VA vs L**.  
4. Comment on the results.  

---

## 🧮 Analysis 2: Extracting κ (Kappa) in Weak Inversion (Subthreshold)

1. Propose **two methods** to determine the **kappa (κ)** value of an nMOS with:  
W = [6, 12, 18, 24] μm
L = 6 μm

2. For each method:  
- Design the schematic setups and perform the required simulations.  
- Conduct the analysis (hand calculations and/or MATLAB) to extract κ.  

3. Compare the κ values obtained by both methods.  

---

