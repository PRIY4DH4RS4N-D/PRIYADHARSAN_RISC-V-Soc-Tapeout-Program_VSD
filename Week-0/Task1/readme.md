<!--
   ╔═══════════════════════════════════════════════════════════╗
   ║     VSD RISC-V Tapeout Program – LECTURE 0 SNAPSHOT      ║
   ╚═══════════════════════════════════════════════════════════╝
   Author: PRIY4DH4RS4N-D
-->

<p align="center">
  <p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=29&duration=2000&pause=1000&color=FF3700&center=true&vCenter=true&width=900&lines=The+RISC-V+SoC+Flow%3A+From+C+to+Silicon!" alt="typing headline"/>
  <br>
  <!-- Animated SVG progress bar to illustrate flow -->
  <img src="https://progress-bar.dev/100/?title=Flow%20from%20C%20to%20Silicon&width=600&color=fd7100" alt=""/>
</p>
  <br>
</p>

---

## 📝 **DOCUMENT OVERVIEW**

> **Instructor:** Kunal Ghosh (VSD - VLSI System Design)  
> **Topic:** RISC-V Tapeout Flow and SoC Integration

---

<div align="center">

### 🛠️ **CHIP MODELLING & RTL FLOW: THE 4-STAGE LAUNCHPAD**

</div>

<div align="center">

<img src="https://skillicons.dev/icons?i=c,verilog" height="40"/> <img src="https://img.shields.io/badge/RTL-Design-blue?style=for-the-badge"/> <img src="https://img.shields.io/badge/Integration-purple?style=for-the-badge"/>

</div>

<table>
<tr>
<td valign="top"><b>🚩 O1: C SPECIFICATION</b></td>
<td>
  <ul>
    <li>System described in <b>C language</b></li>
    <li>Testbenches also in C for early validation</li>
  </ul>
</td>
</tr>
<tr>
<td valign="top"><b>💾 O2: RTL ARCHITECTURE</b></td>
<td>
  <ul>
    <li>Hardware described at RTL using <b>Verilog</b></li>
    <li>Processor & Peripherals/IPs modeled in RTL ("soft copy")</li>
  </ul>
</td>
</tr>
<tr>
<td valign="top"><b>🔄 O3: SOC INTEGRATION</b></td>
<td>
  <ul>
    <li>Integrate processor, peripherals, digital & analog IPs</li>
    <li>Gate-level netlist generated post-synthesis</li>
    <li>Analog IPs/macros hardened as <b>hard macros (HM)</b></li>
  </ul>
</td>
</tr>
</table>

---

<div align="center">

### ⚡ ASIC FLOW: RTL ➡️ GDSII  
</div>

<pre>
Synthesis → Floorplanning → Placement → CTS → Routing
    ↓
 <b>GDSII</b> (final chip database)
    ↓
DRC / LVS (design & layout checks)
</pre>

---

<div align="center">

## 🏁 FINAL SOC & APPLICATIONS

</div>

```diff
+ O4: Final Chip Realization
    • SoC runs at real frequency (100–130 MHz)
    • Same C testbench reused for silicon validation
    • O1 = O2 = O3 = O4 → Consistency from spec to chip!
```

<table>
<tr>
<td>⌚</td><td>iWatch (Wearables)</td>
</tr>
<tr>
<td>💡</td><td>Arduino Boards (Development)</td>
</tr>
<tr>
<td>🖥️</td><td>TV Panels (Consumer Electronics)</td>
</tr>
<tr>
<td>❄️</td><td>AC Applications (Embedded Controllers)</td>
</tr>
</table>

---

<div align="center">

<img src="https://img.shields.io/badge/KEY%20TAKEAWAYS-FFD700?style=for-the-badge&logoColor=white"/>

</div>

- 🧩 **Unified C testbench** = seamless validation across all stages
- 🛤️ **SoC design flow:** C spec → RTL (Verilog) → SoC → GDSII
- 🧪 **Verification at every stage** ensures correctness
- 🌏 **RISC-V SoCs**: powering real-world devices from wearables to industrial controllers

---

<div align="center">
  <img src="https://img.shields.io/badge/Summary%20crafted%20by-PRIY4DH4RS4N--D-1f1f1f?style=for-the-badge"/>
</div>
