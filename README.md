# Alarm-Clock-Digital-Design

#  Alarm Clock System

##  Overview  
This project implements a **modular alarm clock system** in **SystemVerilog**. The design includes core timekeeping, alarm functionality, and advanced features like **weekend detection** and **seven-segment display support**.  

 **Part 1** - Basic alarm clock implementation.  
 **Part 2** - Extended logic, including date display.  
 **Part 3** - Final integration and testing with LCD output.  

##  Features  
- **Basic Alarm Clock** – Allows users to set an alarm and triggers when the time matches.  
- **Day and Week Tracking** – Handles correct modulus operations for days/weeks.  
- **Seven-Segment Display** – Displays time, day, and month using segmented output.  
- **Weekend Detection** – Uses `Alarmon` to differentiate between weekdays and weekends.  
- **LCD Interface** – Manages the visual output for time and alarm status.  

---

##  File Structure  
### **Part 1**  
| File | Description |  
|------|------------|  
| `alarm.sv` | Implements the core alarm clock logic. |  
| `ct_mod_N.sv` | Counter logic with modulo operations. |  
| `lcd_int3.sv` | LCD interface module for display. |  
| `Top_Level.sv` | The top-level module integrating all components. |  
| `output1.txt` | Sample seven-segment display output. |  

### **Part 2 & 3**  
| File | Description |  
|------|------------|  
| `alarm.sv` | Updated alarm logic with additional features. |  
| `ct_mod_N.sv` | Enhanced counter logic. |  
| `lcd_int3.sv` | Updated LCD interface for new display features. |  
| `Top_Level.sv` | The integrated module for final testing. |  
| `output2.txt` | Final output verification. |  

---

##  Simulation & Testing  
### **Requirements**  
- **SystemVerilog Compiler** (ModelSim, QuestaSim, Xilinx Vivado, or similar)  
- **Testbench** to verify correct behavior  

### **Running the Simulation**  
1️⃣ **Compile the SystemVerilog files**  
```sh
vlog alarm.sv ct_mod_N.sv lcd_int3.sv Top_Level.sv
```  
2️⃣ **Run the simulation**  
```sh
vsim -c -do "run -all" Top_Level
```  
3️⃣ **Check the waveform output** or **verify text outputs** (`output1.txt` and `output2.txt`).  

---

##  Contributors  
- **Joachim Galil**  
- **Sean King**  
