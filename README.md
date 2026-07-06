# Analog-Design-of-Low-Dropout-Regulator-LDO-in-45nm-CMOS
# Analog Design of Low Dropout Regulator (LDO) in 45nm CMOS

---

## 📌 Project Overview

This project presents the complete analog IC design flow of a PMOS-based Low Dropout Regulator (LDO) implemented in 45nm CMOS technology using Cadence Virtuoso.

The project includes:

- Transistor-level schematic design
- DC and Transient simulation
- Layout implementation
- DRC verification
- LVS verification
- Parasitic RC extraction (Quantus)
- Post-layout validation

---

## 🎯 Key Specifications

| Parameter | Value |
|-----------|--------|
| Technology | 45nm CMOS |
| Output Voltage | 2.45 V |
| Load Current | ~49 µA |
| PSRR | 13.62 dB |
| Architecture | PMOS Pass Transistor |
| Compensation | Internal Miller Compensation |

---

# 🧠 Architecture

The LDO consists of:

- Reference Voltage Generator  
- Folded Cascode Error Amplifier  
- PMOS Pass Transistor  
- Feedback Divider Network  
- Internal Compensation Network  

---

# 📊 Simulation Results

---

## 🔹 Error Amplifier Schematic

<img src="Results/Error Amplifier Schematic.jpg" width="750">

---

## 🔹 Complete LDO Schematic

<img src="Results/LDO Schematic.jpg" width="750">

---

## 🔹 Transient Response Analysis

<img src="Results/Transient Response Analysis.jpg" width="750">

### Observation:
- Smooth startup behavior
- No overshoot
- Output settles near **2.45 V**
- Stable compensation
- Minimal ripple in steady-state

---

## 🔹 DC Sweep Analysis

<img src="Results/DC Response.jpg" width="750">

### Observation:
- Linear rise initially
- Proper dropout transition
- Stable regulation once Vin > Vout + Vdrop
- No discontinuities

---

# 🧱 Physical Layout & Verification

---

## 🔹 LDO Layout Design

<img src="Results/LDO Layout Design.jpg" width="750">

---

## 🔹 DRC Check

<img src="Results/DRC Check.jpg" width="750">

✔ No Design Rule Violations  
✔ Layout meets 45nm PDK constraints  

---

## 🔹 LVS Match

<img src="Results/LVS Match.jpg" width="750">

✔ Layout matches schematic  
✔ No shorts or opens  

---

## 🔹 Quantus RC Extraction

<img src="Results/Quantus Run.jpg" width="750">

---

## 🔹 RC Extracted Layout

<img src="Results/RC Extraction.jpg" width="750">

✔ Parasitic resistances included  
✔ Parasitic capacitances included  
✔ Post-layout stability verified  

---

# 📐 Performance Analysis

## PSRR Calculation

PSRR = 20 log (VR_supply / VR_out)

Calculated PSRR:

**13.62 dB**

---

## Power Dissipation

Using:

Pd = Vin × Iin

Calculated:

**≈ 0.125 W**

Both analytical and simulation results matched.

---

# 🛠 Tools Used

- Cadence Virtuoso
- Spectre Simulator
- ADE
- Assura DRC/LVS
- Quantus QRC

---

# 📈 Applications

- SoC Power Management
- IoT Devices
- RF Circuits
- Mixed-Signal ICs
- Low Power Systems

---

# 🏆 Project Highlights

✔ Complete Custom Analog IC Flow  
✔ 45nm CMOS Technology Experience  
✔ DRC Clean  
✔ LVS Match  
✔ Post-layout Validation  
✔ Fabrication-ready Layout  

---

## 👨‍💻 Authors

Abhishek H J  
Anirudh H S  
Hemanth Kumar M M  

---
