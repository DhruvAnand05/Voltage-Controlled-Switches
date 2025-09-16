# 🔀 Voltage-Controlled Switches – ELECENG 2EI4 (McMaster University)

## 📖 Project Overview  
This project explores **voltage-controlled switches**, designed and tested for McMaster University’s **ELECENG 2EI4** course.  
The work involved analyzing **ideal switch properties**, implementing MOSFET-based designs, and studying **non-idealities** such as:  
- On-resistance (Ron ≠ 0)  
- Leakage current (Ioff ≠ 0)  
- Voltage limits  
- Non-bidirectional behavior  

Both **PSpice simulations** and **physical hardware testing** with the **Analog Discovery 3 (AD3)** were used to verify performance.  

---

## 🛠️ Tools & Components  
- **OrCAD PSpice** – Circuit design & transient simulations  
- **Analog Discovery 3 (AD3)** – Measurement and analysis  
- **WaveForms Software** – Capturing input/output waveforms  
- **MOSFETs, Voltage Sources, Resistors**  

---

## 🔍 Design & Testing  
Two switch designs were created, each with trade-offs in **complexity, cost, and isolation**:  

### **Switch 1**  
- Used **4 MOSFETs, 3 voltage sources, 1 load resistor**  
- Verified non-idealities: Ron, leakage, threshold voltage, bidirectionality  
- Trade-off: simpler than Switch 2 but still costly  

### **Switch 2**  
- Used **6 MOSFETs, 3 voltage sources, 2 load resistors**  
- Allowed switching between two outputs  
- Trade-off: more complex and costly, but met requirements  

---

## 📊 Simulation Results (PSpice)  
- Output Voltage (on): ~**2.73V** (from 3V input) → confirms **Ron ≠ 0**  
- Leakage Current (off): ~**6.02 pA** → confirms **Ioff ≠ 0**  
- Threshold Voltage: ~**1.75V** → unintended behavior below this range  
- Non-bidirectionality confirmed when reversing load/input  

---

## 🔬 Physical Implementation & Testing  
- Built both switches on a breadboard  
- Measured with **AD3 + WaveForms**  
- Output ~**2.70–2.71V**, matching simulations  
- Leakage current too small for AD3 to measure (≈0A)  
- Non-bidirectionality observed in hardware as well  

---

## 🚀 Key Learnings  
- Real switches deviate significantly from **ideal behavior**  
- MOSFET threshold voltage defines safe operating range  
- Trade-offs exist between **complexity, cost, and performance**  
- Measurement tools (AD3) have limits when capturing very small currents  

---

## 📚 References  
1. O. Ahmed – *Lecture 2*  
2. MathWorks – *Ideal Switch Documentation*  
3. Fluke – *Leakage Current Measurement Basics*  
4. Vishay – *Application Note AN861*  

---

✍️ **Author:** Dhruv Anand  
📅 **Date:** February 2025  
