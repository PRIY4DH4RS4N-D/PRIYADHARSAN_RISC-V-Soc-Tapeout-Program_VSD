# PRIY4DH4RS4N-D-PRIY4DH4RS4N-D-PRIYADHARSAN_RISC-V-Soc-Tapeout-Program_VSD
The VSD RISC-V Tapeout Program, led by Kunal Ghosh, is an open-source VLSI training initiative that teaches end-to-end chip design. It covers the flow from C specification to RTL design, SoC integration, and final GDSII tapeout, using the Sky130 PDK and open-source tools, with applications in real-world devices.

# Week 0: Introduction & Setup

- Introduction to the *VSD RISC-V Tapeout Program* by Kunal Ghosh.  
- Overview of the *chip design and tapeout flow* (O1 → O4 stages).  
- Learned how specifications (C model) evolve into RTL, SoC integration, and final silicon.  
- Understood importance of *C testbench reuse* across all stages.  
- Real-world examples shown: smartwatches, Arduino boards, TV panels, AC applications.  

# Task 1: VSD RISC-V Tapeout Program – Document Summary

This task involved documenting the theoretical RISC-V tapeout design flow. The core process covers four stages:

- *O1: Specification (C Model):*  
  The chip's function is defined using a C model and testbenches.

- *O2: RTL Architecture (Verilog):*  
  The design is converted into hardware description language (Verilog).

- *O3: SoC Integration:*  
  The processor and peripherals are integrated, creating a gate-level netlist.

- *O4: Final Chip Realization:*  
  A functional SoC is produced, validated with the original C testbench to ensure *O1 = O2 = O3 = O4*.

---

### Applications
The lecture also highlighted real-world applications of these SoCs in devices like:  
- Smartwatches (e.g., iWatch)  
- Arduino boards  
- TV panels  
- AC applications

# Task 2: Installation

- Set up the required *EDA tools and environment* for the RISC-V tapeout flow.  
- Installed and configured packages such as *OpenLane, Magic, Ngspice, Yosys, and Sky130 PDK*.  
- Verified installations by running sample designs and basic test commands.  
- Ensured the environment is ready for synthesis, floorplanning, placement, and routing tasks in upcoming weeks.  

## Tools Installation

#### <ins>All the instructions for installation of required tools can be found here:</ins>

### **System Requirements**
- 6 GB RAM
- 50 GB HDD
- Ubuntu 20.04 or higher
- 4 vCPU

### **Resizing the Ubuntu window to fit the screen**
```bash
$ sudo apt update
$ sudo apt install build-essential dkms linux-headers-$(uname -r)
$ cd /media/spatha/VBox_GAs_7.1.8/
$ ./autorun.sh
```

### **TOOLS TO INSTALL**

#### <ins>**Yosys**</ins>
```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make               # If make is not installed
sudo apt-get install build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
# Yosys build depends on a Git submodule called abc, which hasn't been initialized yet. You need to run the following command before running make
git submodule update --init --recursive
make 
sudo make install
```
### Yosys Verification
![Yosys Verification](Week-0/Task-2/Images-Verification-Of-Installed-tools/1-Yosys-Verified.png)

#### <ins>**Iverilog**</ins>
```bash
sudo apt-get update
sudo apt-get install iverilog
```
### Icarus Verilog Verification
![Icarus Verilog Verification](Week-0/Task-2/Images-Verification-Of-Installed-tools/2-Iverilog-Verified.png)

#### <ins>**gtkwave**</ins>
```bash
sudo apt-get update
sudo apt install gtkwave
```
### GTKWave Verification
![GTKWave Verification](Week-0/Task-2/Images-Verification-Of-Installed-tools/3-gtkwave-Verified.png)
