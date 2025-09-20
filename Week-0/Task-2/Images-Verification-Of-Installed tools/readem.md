<!--
 ██████████████████████████████████████████████████████████████████████████
 █─▄▄▄▄█▄─▄█▄─█─▄█▄─▄▄─█▄─▄▄▀█▄─▄▄─█▄─▄▄─█▄─▄▄▀█▄─▄█▄─▄▄─█▄─▄█─▄▄─█▄─▄▄▀█
 █▄▄▄▄─██─███▄▀▄███─▄█▀██─▄─▄██─▄█▀██─▄█▀██─▄─▄██─███─▄█▀██─██─██─██─▄─▄█
 ▀▄▄▄▄▄▀▄▄▄▀▀▀▄▀▀▀▄▄▄▄▄▀▄▄▀▄▄▀▄▄▄▄▄▀▄▄▄▄▄▀▄▄▀▄▄▀▄▄▄▀▄▄▄▄▄▀▄▄▄▀▄▄▄▄▀▄▄▀▄▄▀
-->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:3b82f6,100:fbbf24&height=90&section=header&text=RISC-V%20SoC%20TAPEOUT%20TOOLKIT%20SETUP&fontAlign=50&fontSize=37&fontColor=fff" width="100%">

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=25&pause=1100&color=FFD700&center=true&vCenter=true&width=900&lines=YOUR+GATEWAY+TO+THE+RISC-V+EDA+UNIVERSE!" alt="headline" />
</div>

---

Welcome, fellow silicon explorer!  
This **uniquely visual guide** helps you install and verify all the vital open-source EDA tools for your RISC-V SoC tapeout journey.  
Every tool section features:

- 🚀 **Install Command**
- 🖼️ **Real Verification Screenshot (from my setup)**

---

## 1. 🎩 Yosys — _Synthesis Wizard_

**Install Command**
```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make (If make is not installed please install it)
sudo apt-get install build-essential clang bison flex \
libreadline-dev gawk tcl-dev libffi-dev git \
graphviz xdot pkg-config python3 libboost-system-dev \
libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install
```
**Verify**
```bash
yosys
```
<img src="./1-Yosys.png" alt="Yosys verification" width="72%" />

---

## 2. ⚙️ Icarus Verilog — _Simulation Engine_

**Install Command**
```bash
sudo apt-get update
sudo apt-get install iverilog
```
**Verify**
```bash
iverilog
```
<img src="./2-Iverilog.png" alt="Icarus Verilog verification" width="72%" />

---

## 3. 🌊 GTKWave — _Waveform Explorer_

**Install Command**
```bash
sudo apt-get update
sudo apt install gtkwave
```
**Verify**
```bash
gtkwave
```
<img src="./3-Gtkwave.png" alt="GTKWave verification" width="72%" />

---

## 4. ⚡ Ngspice — _Analog/Mixed-Signal Sim_

**Install Command**
```bash
tar -zxvf ngspice-37.tar.gz
cd ngspice-37
mkdir release
cd release
../configure --with-x --with-readline=yes --disable-debug
make
sudo make install
```
**Verify**
```bash
ngspice
```
<img src="./4-ngspice.png" alt="Ngspice verification" width="72%" />

---

## 5. 🧙‍♂️ Magic VLSI — _Layout Magician_

**Install Command**
```bash
sudo apt-get install m4
sudo apt-get install tcsh
sudo apt-get install csh
sudo apt-get install libx11-dev
sudo apt-get install tcl-dev tk-dev
sudo apt-get install libcairo2-dev
sudo apt-get install mesa-common-dev libglu1-mesa-dev
sudo apt-get install libncurses-dev
git clone https://github.com/RTimothyEdwards/magic
cd magic
./configure
make
make install
```
**Verify**
```bash
magic
```
<img src="./5-Magic.png" alt="Magic verification" width="72%" />

---

<div align="center">
  <img src="https://img.shields.io/badge/All%20Tools-READY-success?style=for-the-badge&logo=vercel"/>
</div>

---

## 🏁 Final Checklist

- If each tool launches and looks like the screenshots above, your EDA environment is ready for RTL ✈️ GDSII!
- These open-source supertools span **synthesis, simulation, waveforms, analog, and layout**—the full chip design arsenal.

---

<div align="center">
  <img src="https://img.shields.io/badge/Happy%20Silicon%20Crafting!-black?style=for-the-badge"/>
  <br><br>
  <sub>Guide & screenshots curated by <a href="https://github.com/PRIY4DH4RS4N-D">PRIY4DH4RS4N-D</a></sub>
</div>
