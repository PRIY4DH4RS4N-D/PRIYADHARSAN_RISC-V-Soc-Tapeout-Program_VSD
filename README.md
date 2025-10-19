<!--
██████╗ ██████╗ ██╗██████╗  █████╗ ██╗   ██╗
██╔══██╗██╔══██╗██║██╔══██╗██╔══██╗██║   ██║
██████╔╝██████╔╝██║██║  ██║███████║██║   ██║
██╔═══╝ ██╔══██╗██║██║  ██║██╔══██║██║   ██║
██║     ██║  ██║██║██████╔╝██║  ██║╚██████╔╝
╚═╝     ╚═╝  ╚═╝╚═╝╚═════╝ ╚═╝  ╚═╝ ╚═════╝
-->

<div align="center">


<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=105&section=header&text=RISC-V+SoC+Tapeout+Program+VSD&fontSize=38&fontColor=F7F7F7" width="100%">


<p>
  <img src="https://img.shields.io/badge/RISC--V-SoC%20Tapeout-1976d2?style=for-the-badge&logo=riscv"/>
  <img src="https://img.shields.io/badge/VSD-Program-ff9800?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Participants-3500%2B-43a047?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Made%20in-India-fcba03?style=for-the-badge"/>
</p>

</div>

---

<div align="center">

## 🚩 _**LOGIC TO LAYOUT: ADVANCING INDIA’S SEMICONDUCTOR DESIGN**!_

</div>

---

<div align="center">
  
> **"This repo is my vibrant logbook for the SoC Tapeout Program (VSD): an odyssey from RTL to GDSII using open-source EDA. Join the 3500+ strong cohort building silicon, fueling India's semiconductor dream!"**

</div>

---


## 📝 Repo Overview

This repository captures the **hands-on journey of building, simulating, synthesizing, and analyzing a minimal RISC-V SoC** (BabySoC) using **open-source tools** and **Sky130 PDK technology**.  
It spans **RTL design**, **Gate-Level Simulation (GLS)**, **Static Timing Analysis (STA)**, and **CMOS circuit-level experiments**, bridging **digital hardware design** with **device physics and timing analysis**.

**Tools & Frameworks Used:**
- **RTL & Simulation:** Verilog, Icarus Verilog, GTKWave  
- **Synthesis & GLS:** Yosys, ABC, OpenSTA  
- **Technology:** Sky130 PDK, Standard Cell Libraries  
- **SPICE Analysis:** NMOS/CMOS characterization, transient simulations

---

## 📅 Week-wise Summary

| Week | Focus Area | Key Achievements |
|------|------------|-----------------|
| **Week 1** | RTL Design & Simulation | - Learned Verilog basics<br>- Simulated MUX, DEMUX, RCA<br>- Gate-level synthesis using Yosys<br>- Identified RTL coding pitfalls (blocking/non-blocking, sensitivity lists, incomplete if/case) |
| **Week 2** | Minimal SoC Integration | - Set up VSDBabySoC environment<br>- Verified RVMYTH CPU, PLL, DAC<br>- Pre-synthesis simulations and waveform analysis<br>- RTL-to-Verilog TLV conversion |
| **Week 3** | Gate-Level Simulation & STA | - Post-synthesis functional verification<br>- Gate-level simulations with SDF delays<br>- Timing checks using OpenSTA across PVT corners<br>- Slack analysis, setup/hold checks, timing reports |
| **Week 4** | CMOS Device Characterization | - NMOS I-V curves, threshold extraction<br>- CMOS inverter analysis and VTC<br>- Noise margin calculation (NML/NMH)<br>- Variation studies (Vdd scaling, W/L ratio)<br>- STA correlation with device-level behavior |

---

## ✅ Overall Checklist of Completed Tasks

- [x] **RTL Design**: MUX, RCA, blocking/non-blocking labs  
- [x] **Simulation**: Icarus Verilog, GTKWave waveform verification  
- [x] **Synthesis**: Yosys synthesis, ABC mapping, post-processing  
- [x] **Gate-Level Simulation**: GLS with delays, verification against RTL  
- [x] **Static Timing Analysis**: Setup/Hold checks, slack reports, PVT corners  
- [x] **BabySoC Integration**: RVMYTH CPU, DAC, PLL functional verification  
- [x] **TL-Verilog Conversion**: TLV → Verilog for CPU core  
- [x] **CMOS Device Analysis**: I-V curves, threshold extraction, VTC, delay, noise margins  
- [x] **Variation Studies**: W/L ratio, Vdd scaling, environmental effects  
- [x] **Documentation**: Annotated plots, summary tables, weekly reports  

---

## 📂 Repo Structure

```txt
VSDBabySoC/
├── Week1_RTL/            # RTL design, simulation, synthesis examples
├── Week2_SoC/            # BabySoC setup, TLV→Verilog conversion, DAC/PLL tests
├── Week3_GLS_STA/        # Gate-level simulation, OpenSTA timing analysis
├── Week4_CMOS/           # SPICE simulations, inverter analysis, variation studies
├── Images/               # Waveforms, netlists, STA plots
├── References.md         # External tutorials, libraries, tool links
└── README.md             # Overview & progress tracker

```

## 🔗 Program Links

<p align="center">
  <a href="https://vsdiat.vlsisystemdesign.com/"><img src="https://img.shields.io/badge/VSD-Official%20Website-1976d2?style=for-the-badge"/></a>
  <a href="https://riscv.org/"><img src="https://img.shields.io/badge/RISC--V-International-43a047?style=for-the-badge"/></a>
  <a href="https://efabless.com/"><img src="https://img.shields.io/badge/Efabless-Platform-f4511e?style=for-the-badge"/></a>
</p>

<div align="center">

### 👨‍💻 Crafted with 💡 by [PRIY4DH4RS4N-D](https://github.com/PRIY4DH4RS4N-D)

</div>
