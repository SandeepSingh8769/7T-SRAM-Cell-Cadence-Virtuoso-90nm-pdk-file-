<h1 align="center">7T SRAM Cell Design using Cadence Virtuoso (90nm)</h1>
<p align="center"><b>Low-Power • High Stability • Read-Disturb Free</b></p>
# Design and Analysis of 7T SRAM Cell using Cadence Virtuoso

## 📌 Overview
Static Random Access Memory (SRAM) is widely used in high-speed and low-power VLSI systems. Conventional 6T SRAM cells suffer from read disturb issues, reduced static noise margin (SNM), and higher leakage at scaled technologies.  

This project presents the design and analysis of a **7T SRAM cell** using Cadence Virtuoso in **90 nm CMOS technology**. The additional transistor separates the read and write paths, improving read stability and reducing power consumption.

---

## 🎯 Objectives
- Design transistor-level 7T SRAM cell  
- Analyze write, read, and hold operations  
- Improve static noise margin (SNM)  
- Reduce dynamic power consumption  
- Compare performance with conventional 6T SRAM  

---

## 🧠 7T SRAM Architecture
The proposed 7T SRAM cell consists of:

- Two cross-coupled CMOS inverters (storage latch)  
- One write access transistor  
- Dedicated read path transistors  

The key concept is **decoupling of read and write paths**, which eliminates read disturb and improves stability.

---

## ⚙️ Modes of Operation

### 🔹 Hold Mode
- WL = LOW  
- RWL = LOW  
- Cross-coupled inverters retain data  
- Very low leakage and high stability  

### 🔹 Write Operation
- WL = HIGH  
- Input data overwrites stored value  
- Q and Q̅ update correctly  

### 🔹 Read Operation
- RWL = HIGH  
- Read bit line responds to stored data  
- Internal nodes remain undisturbed  

---

## 🛠 Tools and Technology
- Cadence Virtuoso  
- ADE L (Transient Analysis)  
- **90 nm CMOS PDK**  
- Supply Voltage: 1.8 V  

---

## 📈 Simulation Results
Transient simulations verify:

- ✅ Successful write operation  
- ✅ Stable hold operation  
- ✅ Disturb-free read operation  
- ✅ Improved reliability over 6T SRAM  

The isolation of the read path prevents disturbance of the stored data and enhances overall cell stability.

---

## 📊 6T vs 7T SRAM (Key Improvements)

| Parameter | 6T SRAM | 7T SRAM |
|----------|--------|--------|
| Read disturb | Present | Eliminated |
| Read stability | Lower | Higher |
| Dynamic power | Higher | Lower |
| Leakage | Higher | Reduced |
| Reliability | Moderate | Improved |
| Area | Smaller | Slightly larger |

---

## 🚀 Applications
- Cache memory in processors  
- Register files  
- Low-power embedded systems  
- System-on-Chip (SoC)  
- IoT devices  
- AI/ML accelerators  

---

## 🔮 Future Scope
- Layout design with DRC/LVS  
- SRAM array implementation  
- Technology scaling (45 nm / FinFET)  
- Monte Carlo variation analysis  
- Power optimization techniques  

---

## 👨‍💻 Authors
**Sandeep Singh**  

---

⭐ If you find this project useful, please give it a star!
