# Day 4: CMOS Inverter Noise Margin Analysis

## 🔍 Objective
To analyze the **noise margins** of a **CMOS inverter** using SPICE simulation with specified device parameters and capacitive load.

---

## ⚙️ Device Parameters
- **Technology:** Sky130 (1.8 V)
- **PMOS Width (Wp):** 1 µm  
- **NMOS Width (Wn):** 0.36 µm  
- **Load Capacitance (CL):** 50 fF  

---

## 🧪 Analysis
- Perform a **DC sweep** of input voltage (**Vin**) from 0 V to 1.8 V.  
- Observe the **Voltage Transfer Characteristics (VTC)** curve to determine:
  - **VOH (logic high output voltage)**  
  - **VOL (logic low output voltage)**  

<img src="./IMAGES/30.png" width="550">

**Key Observations:**  
- For **Vin < ~0.7 V**, **Vout ≈ 1.8 V** → Output is logic **‘1’**.  
- For **Vin > ~1.0 V**, **Vout ≈ 0 V** → Output is logic **‘0’**.

---

## 🧠 Summary
This experiment focuses on finding the **noise margins** of the CMOS inverter, which define its **tolerance to input noise** while maintaining correct logic levels.  
The results show clear **switching regions** and help determine **NMH** and **NML**, essential for ensuring **robust digital circuit operation**.
