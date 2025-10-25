

---

# 🗓️ Week 5 – OpenROAD Flow: Floorplanning & Cell Placement

## 🎯 Goal

This week's focus is on executing the OpenROAD flow to produce a layout that includes both floorplanning and standard cell placement. Key tasks include:

- Preparing the OpenROAD software environment  
- Running automated flow scripts  
- Viewing the resulting layout using the graphical interface  

---

## ⚙️ Step 1: Installing OpenROAD

### 📥 Clone the Flow Scripts Repository
```bash
git clone https://github.com/The-OpenROAD-Project/OpenROAD-flow-scripts.git
cd OpenROAD-flow-scripts
```

### 🧰 Run Setup Script
```bash
sudo ./setup.sh
```

### 🏗️ Build the OpenROAD Tool Locally
```bash
./build_openroad.sh --local
```

### ✅ Confirm Environment Configuration
```bash
source ./env.sh
openroad -help
```

![im1](im1.png)

---

## 📐 Step 2: Executing the Flow & Launching GUI

### 📁 Enter the Design Flow Directory
```bash
cd <path-to-makefile-flow-directory>
make
```

### 🖥️ Open GUI for Final Layout Inspection
```bash
make gui_final
```

![im2](im2.png)

### 🔍 GUI Highlights
- Floorplan successfully generated for the `gcd` design block  
- Standard cells are placed across the core region  
- Wire routing and interconnects are visible in the 2D view  

### 📜 Terminal Output Includes
- `Floorplan stage completed`  
- `Placement stage completed`  
- `Core area: <value>`  
- `Die dimensions: <value>`  

---

## 🧾 Recap

- OpenROAD environment was installed and verified  
- Flow executed using `make gui_final`  
- Floorplan and placement stages completed successfully  
- Layout verified visually and via terminal logs  

---



