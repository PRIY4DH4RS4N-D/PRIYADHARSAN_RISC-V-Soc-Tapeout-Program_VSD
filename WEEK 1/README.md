<!--
██████╗ ██████╗ ██╗██████╗  █████╗ ██╗   ██╗
██╔══██╗██╔══██╗██║██╔══██╗██╔══██╗██║   ██║
██████╔╝██████╔╝██║██║  ██║███████║██║   ██║
██╔═══╝ ██╔══██╗██║██║  ██║██╔══██║██║   ██║
██║     ██║  ██║██║██████╔╝██║  ██║╚██████╔╝
╚═╝     ╚═╝  ╚═╝╚═╝╚═════╝ ╚═╝  ╚═╝ ╚═════╝
-->
<div align="center">
  
<img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=105&section=header&text=RISC-V%20Reference%20SoC%20Tapeout%20Program%20VSD&fontSize=38&fontAlign=50&fontColor=F7F7F7" width="100%">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Mono&size=28&pause=1200&color=FFB300&center=true&vCenter=true&width=800&lines=RTLDesign+%E2%9E%9E+Synthesis+%E2%9E%9E+PhysicalDesign+%E2%9E%9E+Tapeout" alt="pipeline" />

<p>
  <img src="https://img.shields.io/badge/RISC--V-SoC%20Tapeout-1976d2?style=for-the-badge&logo=riscv"/>
  <img src="https://img.shields.io/badge/VSD-Program-ff9800?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Participants-3500%2B-43a047?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Made%20in-India-fcba03?style=for-the-badge"/>
</p>
</div>

---
<div align="center">

## 🚩 _**RTL to Gates: My Week 1 Digital Design Journey!**_

</div>

---

<div align="center">
  
> **"This week marks my hands-on entry into open-source digital hardware design. From simulating Verilog to synthesizing and verifying at the gate level—every day built my foundation for SoC and VLSI innovation!"**

</div>

---

## 🧭 Quick Nav

- **WEEK 1 OVERVIEW**
- **DAY-WISE JOURNAL**
- **KNOWLEDGE TABLES**
- **FLOW DIAGRAM**
- **KEY TAKEAWAYS**
- **ACKNOWLEDGMENTS**

---

## 📅 Week 1 — RTL Design & Synthesis

<details>
<summary><b>📘 Day 1: RTL Design & Simulation Basics</b></summary>

- [🔹 Verilog & Tools Intro](./Day1/Intro.md)
- [🔹 2:1 MUX – Code & Simulation](./Day1/mux2x1.v)
- [🔹 GTKWave Output](./Day1/Images/mux_waveform.png)
- [🔹 Yosys Synthesis Flow](./Day1/yosys_flow.md)
</details>

<details>
<summary><b>📘 Day 2: Logic Synthesis & Gate-level Simulation</b></summary>

- [🔹 Yosys Synthesis](./Day2/synthesis.md)
- [🔹 Gate-Level Simulation (GLS)](./Day2/gls.md)
- [🔹 Inferred Latch Example](./Day2/inferred_latch.v)
- [🔹 Observations & Waveforms](./Day2/Images/)
</details>

<details>
<summary><b>📘 Day 3: Blocking vs Non-blocking, Sensitivity Lists</b></summary>

- [🔹 Blocking vs Non-blocking](./Day3/blocking_nonblocking.v)
- [🔹 Sensitivity List Mismatches](./Day3/sensitivity_list.v)
- [🔹 Simulation vs Synthesis Labs](./Day3/labs.md)
- [🔹 GTKWave Examples](./Day3/Images/)
</details>

<details>
<summary><b>📘 Day 4: If-Else & Case Constructs</b></summary>

- [🔹 Priority Logic with If-Else](./Day4/if_else.v)
- [🔹 Case Statement MUX](./Day4/case_mux.v)
- [🔹 Incomplete If/Case Issues](./Day4/incomplete_if_case.md)
- [🔹 Labs & Netlists](./Day4/Images/)
</details>

<details>
<summary><b>📘 Day 5: Synthesis Optimization & Coding Pitfalls</b></summary>

- [🔹 Incomplete If/Case Labs](./Day5/incomp_if.v)
- [🔹 Overlapping Case Labs](./Day5/bad_case.v)
- [🔹 Procedural For Loop](./Day5/mux32x1.v)
- [🔹 Generate Loop for RCA](./Day5/rca_generate.v)
- [🔹 Ripple Carry Adder](./Day5/rca.v)
- [🔹 Labs & Netlists](./Day5/Images/)
- [🔹 Day 5 Recap](./Day5/summary.md)
</details>

---

## 🏷️ Quick Access

- 📄 [Full Week 1 Summary](./Week1_Summary.md)
- 🖼️ [All Images](./Images/)
- 📚 [References](./References.md)

---

## 🌟 Week 1 – Highlight Reel

### Day 1: **RTL Simulation Flow**
- 🚀 Explored **Icarus Verilog → GTKWave** workflow.
- 🛠️ Designed and simulated a **2:1 MUX**.
- 🎯 *Key*: Visualize RTL behavior before hardware mapping!

### Day 2: **RTL to Gates**
- 🏗️ Synthesized designs with **Yosys**.
- 🔬 Compared **RTL code** to **netlist hardware**.
- 💡 *Insight*: Synthesis = mapping logic to real gates.

### Day 3: **GLS & Coding Mismatches**
- 🔄 Ran **GLS** (Gate-Level Simulation).
- 🕵️ Identified **simulation-synthesis mismatches**.
- ⚠️ Bad sensitivity lists or blocking = bugs!

### Day 4: **RTL Coding Caveats**
- 🧩 Compared **if-else** vs **case** for logic.
- 🩹 Caught **latch inference** & mismatches.
- 🚨 *Lesson*: Small code mistakes, big hardware problems!

### Day 5: **Optimization Masterclass**
- 🟢 Saw how **incomplete if/case** infer latches.
- 🔁 Explored **for loops**: procedural vs generate.
- ⚡ Built scalable designs (MUXes, RCA) with `generate`.

---

## 📊 Knowledge Tables

#### If vs Case

| Feature              | `if-else` (Priority) | `case` (Multiplexer) |
|----------------------|----------------------|----------------------|
| Synthesized As       | MUX chain            | Multiplexer          |
| Use Case             | Priority logic       | Clean, scalable      |
| Caveat               | Missing else → latch | Overlaps → undefined |

---

#### Procedural vs Generate Loops

| Feature         | Procedural `for` | `generate for` |
|-----------------|------------------|---------------|
| Where?          | Inside `always`  | Outside `always` |
| Purpose         | Model behavior   | Structure/replicate hardware |
| Example         | Testbenches, sequential logic | MUX, adders, busses |

---

## 🔄 RTL to GDSII Flow

```plaintext
Verilog RTL
   │
   ▼
Simulation (Icarus) ──▶ Waveform (GTKWave)
   │
   ▼
Synthesis (Yosys) ──▶ Netlist
   │
   ▼
Gate-Level Simulation (GLS)
```

---

## 🏁 What I Gained

- 🧩 **End-to-end digital flow:** RTL → Simulation → Synthesis → GLS
- 🕵️ **Pitfall hunting:** incomplete if/case, blocking/non-blocking, sensitivity list issues
- 🧪 **Hands-on labs:** MUX, DEMUX, RCA – built & simulated
- 🚦 **Open-source EDA confidence:** Icarus, GTKWave, Yosys
- 💡 **Big takeaway:** _Clean, complete RTL code = reliable hardware!_

---

## 🙏 Acknowledgment

> **Thanks to [Kunal Ghosh](https://github.com/kunalg123) and the [VSD Team](https://vsdiat.vlsisystemdesign.com/) for pioneering open-source VLSI education.**

---

## 📚 References

1. [Icarus Verilog](http://iverilog.icarus.com/) – Simulation  
2. [GTKWave](http://gtkwave.sourceforge.net/) – Waveform Viewer  
3. [Yosys HQ](https://yosyshq.net/yosys/) – Synthesis  
4. [Sky130 PDK](https://skywater-pdk.readthedocs.io/) – Open source cell libraries  
5. Sudip Misra NPTEL – *Industry 4.0 and IIoT (Verilog Synthesis Part)*

---

<div align="center">

**👨‍💻 Crafted with passion by [PRIY4DH4RS4N-D](https://github.com/PRIY4DH4RS4N-D)**

</div>
