# WEEK 6
<!-- ██████╗ ██╗███████╗██╗ ██╗██╗ ██████╗ █████╗ ███╗ ██╗ ██╔══██╗██║██╔════╝██║ ██╔╝██║██╔════╝██╔══██╗████╗ ██║ ██║ ██║██║█████╗ █████╔╝ ██║██║ ███████║██╔██╗ ██║ ██║ ██║██║██╔══╝ ██╔═██╗ ██║██║ ██╔══██║██║╚██╗██║ ██████╔╝██║███████╗██║ ██╗██║╚██████╗██║ ██║██║ ╚████║ ╚═════╝ ╚═╝╚══════╝╚═╝ ╚═╝╚═╝ ╚═════╝╚═╝ ╚═╝╚═╝ ╚═══╝ --> <div align="center"> <img src="https://capsule-render.vercel.app/api?type=rect&color=gradient&height=105&section=header&text=RTL-TO-GDSII%20USING%20OPENLANE%20(SKY130%20PDK)&fontSize=38&fontAlign=50&fontColor=F7F7F7" width="100%">
🎯 OBJECTIVE

# Perform the complete RTL-to-GDSII flow for a RISC-V SoC using OpenLANE and Sky130 PDK, covering every stage of physical design, from synthesis to post-layout timing validation.

## 🧩 TASK COMPONENTS
### 1. 🏗️ Design Setup and Floorplanning

Load synthesized netlist into OpenLANE environment

Define die area, core utilization, and placement constraints

Insert I/O pins and establish routing channels

Generate floorplan DEF and visualize in Magic

### 2. 🧱 Placement and Optimization

Run global and detailed placement for standard cells

Optimize placement for wirelength and timing

Verify legal cell positioning and check placement density

Save final placed DEF for next stage

### 3. ⏱️ Clock Tree Synthesis (CTS)

Identify clock nets and insert clock buffers/inverters

Balance clock paths to minimize skew

Generate post-CTS DEF and updated netlist

Validate timing (pre-PDN) using OpenSTA

### 4. ⚡ Power Distribution Network (PDN) Generation

Create power/ground (VDD/VSS) rails and metal straps

Ensure uniform power delivery to all standard cells

Connect clock buffers to PDN grid

Visualize PDN layers and verify continuity in Magic

### 5. 🚀 Routing with TritonRoute

Perform global routing to define path guides

Execute detailed routing to form metal tracks and vias

Use search-and-repair loops to remove DRC violations

Generate final routed DEF and GDS view

### 6. 📏 Design Rule Check (DRC)

Run DRC on final layout to ensure manufacturing compliance

Detect and fix spacing, width, and via errors

Confirm DRC-clean layout ready for parasitic extraction

### 7. 🧮 Parasitic Extraction (SPEF)

Use SPEF extractor to calculate wire R and C values

Generate .spef file containing interconnect parasitics

Prepare extracted data for timing verification

### 8. 🧠 Post-Route Static Timing Analysis (STA)

Load post-route netlist, SPEF, and constraints into OpenSTA

Evaluate setup/hold violations with real interconnect delays

Verify timing closure and signal integrity

### 9. 🧩 Final GDS Export and Verification

Merge all layers to produce final GDSII layout

Cross-check layout in Magic and KLayout

Prepare design for tape-out submission

### 📋 DELIVERABLES

✅ Floorplan, Placement, CTS, and Routing reports

✅ PDN and DRC verification logs

✅ SPEF parasitic file and OpenSTA timing report

✅ Final GDSII layout (DRC-clean, LVS-ready)

✅ Documentation of full flow commands and results

### 🎓 LEARNING OUTCOMES

✅ End-to-end RTL-to-GDSII flow comprehension

✅ Hands-on experience with OpenLANE & OpenROAD tools

✅ Understanding of PDN, CTS, and DRC methodologies

✅ Proficiency in post-layout timing analysis (OpenSTA)

✅ Fabrication-ready design generation using Sky130 PDK

### 💼 PROFESSIONAL SKILLS DEVELOPED

✅ ASIC flow automation and EDA tool usage

✅ Layout debugging and DRC issue resolution

✅ Power and clock network design

✅ Post-route analysis and optimization

✅ Tape-out documentation and reporting
