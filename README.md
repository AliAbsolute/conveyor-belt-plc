# PLC Conveyor Belt Sorting System 🚦

This is my **first PLC simulation project** built with [OpenPLC Editor](https://openplcproject.com/).  
It simulates a simple **conveyor belt sorting system** that can detect large objects and divert them using a gate actuator.

---

## ⚙️ Features
- Motor start/stop circuit with latch
- Emergency stop interlock for safety
- Large-item sensor
- Pulse timer (`TP`) to activate diverter for 3 seconds

## 📋 How It Works
1. Press **Start** → Motor (`M_CONV`) runs and latches on.  
2. Press **Stop** or **E-Stop** → Motor turns off.  
3. When **sensor detects a large item** (`S_LARGE`) while motor is running, a **pulse timer** energizes the diverter (`DIVERT`) for 3 seconds.
   
---

## 🚀 Next Steps
- Add counters (CTU) to track items sorted  
- Add bin-full indicator lamp  
- Expand into multi-sensor systems

---

## 📂 Files
- `Conveyor_Sorter.xml` → PLC program
- `screenshots/` → images of ladder logic & tests
