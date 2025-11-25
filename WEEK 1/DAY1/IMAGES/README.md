<!--
██████╗ ██████╗ ██╗██████╗  █████╗ ██╗   ██╗
██╔══██╗██╔══██╗██║██╔══██╗██╔══██╗██║   ██║
██████╔╝██████╔╝██║██║  ██║███████║██║   ██║
██╔═══╝ ██╔══██╗██║██║  ██║██╔══██║██║   ██║
██║     ██║  ██║██║██████╔╝██║  ██║╚██████╔╝
╚═╝     ╚═╝  ╚═╝╚═╝╚═════╝ ╚═╝  ╚═╝ ╚═════╝
-->

# **DAY 1: RTL DESIGN & SYNTHESIS – INTRODUCTION** 

<span>
  <b>Yosys</b> <kbd>Synthesis</kbd> • <b>Icarus Verilog</b> <kbd>Simulation</kbd> • <b>GTKWave</b> <kbd>Waveform Analysis</kbd>
</span>

</div>

---

## 🎯 **Day 1 Focus**

- Grasp the essentials of RTL simulation using **Icarus Verilog**
- Write and test a **2:1 multiplexer** (MUX) in Verilog
- Dive into **Yosys** for digital logic synthesis

---

## 🧰 **Toolbox Overview**

| **Role**     | **Tool**                 | **Purpose**                         |
|--------------|--------------------------|-------------------------------------|
| Simulator    | Icarus Verilog (iverilog)| Simulate RTL + testbench            |
| Verification | GTKWave                  | Visualize simulation waveforms      |
| Synthesizer  | Yosys                    | Synthesize RTL into a gate netlist  |

---

## 🧭 **Simulation & Synthesis Flow**

1. **Design**: Write Verilog code that implements the required logic (e.g., a 2:1 MUX).
2. **Testbench**: Create a testbench to apply stimulus and verify design outputs.
3. **Simulation**: Use Icarus Verilog to run RTL simulation and generate a `.vcd` (waveform) file.
4. **Waveform Analysis**: Open the `.vcd` in GTKWave to inspect signals and ensure correctness.
5. **Synthesis**: Use Yosys to convert RTL to a gate-level netlist, preparing for hardware realization.
6. **Verification**: Optionally simulate the synthesized netlist to confirm functional equivalence.

---

## 🌐 **Simulation Explained**

**Why simulate?**  
Simulation checks if the design meets its functional requirements before moving to hardware.  
**How?**  
- The testbench applies various input conditions.
- Output signals are monitored for correctness.
- Bugs are detected early—saving time and effort.

---

## 💡 **Key Concepts**

- **Design**: The Verilog module describing the intended logic (e.g., mux, adder, etc.).
- **Testbench**: A special Verilog file that is *not* synthesized, used only to simulate and verify the design.
- **VCD File**: Value Change Dump file, records signal changes for waveform viewing.
- **Synthesis**: The process of translating RTL into a gate-level representation suitable for chip fabrication.
- **Netlist**: A list of logic gates and their interconnections, output of synthesis.

---

## 📝 **Lab Steps**

#### 1️⃣ Clone the Workshop Repository

```sh
git clone https://github.com/kunalg123/sky130RTLDesignAndSynthesisWorkshop.git
cd sky130RTLDesignAndSynthesisWorkshop/verilog_files
```

#### 2️⃣ Compile the Design and Testbench

```sh
iverilog good_mux.v tb_good_mux.v
```
- This produces an executable simulation file (`a.out` by default).

#### 3️⃣ Run the Simulation

```sh
./a.out
```
- This generates a `tb_good_mux.vcd` file for waveform viewing.

#### 4️⃣ View Waveform in GTKWave

```sh
gtkwave tb_good_mux.vcd
```
- Inspect signal transitions and confirm design correctness.

#### 5️⃣ Edit Design and Testbench

```sh
gvim tb_good_mux.v -o good_mux.v
```
- Use your preferred editor to refine code as needed.

#### 6️⃣ Synthesize the Design with Yosys

```sh
yosys
read_liberty -lib ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
read_verilog good_mux.v
synth -top good_mux
abc -liberty ../my_lib/lib/sky130_fd_sc_hd__tt_025C_1v80.lib
show
```
- These commands perform synthesis, optimization, and netlist generation.

---

## 🛠️ **Understanding Gate Library Variants**

A technology library provides multiple versions of each logic gate (AND, OR, etc.), each tailored for:
- **Performance**: Fast cells for speed-critical paths
- **Power**: Low-power cells for efficient operation
- **Area**: Compact cells for smaller chip footprint
- **Drive Strength**: Stronger cells to drive larger loads
- **Signal Integrity**: Cells with enhanced noise tolerance

During synthesis, Yosys selects the most appropriate gate variant for each part of the design according to your constraints (timing, power, etc.).

---

## ✔️ **What Did I Learn Today?**

- The **RTL to gates flow** using only open-source tools.
- How to structure a Verilog project: separate design and testbench files.
- How to simulate, debug, and visualize digital designs.
- The importance of gate libraries and technology mapping during synthesis.
- Hands-on with lab commands, from repo cloning to synthesis.

---

## 📚 **References**

1. [VSD – Sky130 Open Source Tapeout](https://www.vlsisystemdesign.com/vsd-sky130/)
2. [Yosys Open Synthesis Suite](https://yosyshq.readthedocs.io/)
3. [Icarus Verilog](http://iverilog.icarus.com/)
4. [GTKWave](http://gtkwave.sourceforge.net/)

---

<div align="center">

**🚀 Day 1: RTL Simulation & Synthesis — The Open-Source Way!**

</div>
