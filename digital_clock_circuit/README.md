# Digital Clock Circuit (24-Hour Format)

## Overview
This project involves the design, construction, and testing of a fully discrete **digital clock circuit** implemented using small-scale integrated circuits (SSI). The clock displays **hours, minutes, and seconds** in a **24-hour format** using seven-segment displays.

The system was built entirely with **hardware-based digital logic** (no microcontroller), emphasizing fundamental concepts in sequential circuits, timing, and counter design.

---

## Objectives
- Design a digital clock using discrete digital ICs  
- Generate a stable **1 Hz clock signal**  
- Implement seconds, minutes, and hours counting  
- Cascade counters with proper reset logic  
- Drive seven-segment displays using BCD-to-7-segment drivers  
- Validate operation through measurement and observation  

---

## System Description
The clock consists of three main subsystems:

### Seconds and Minutes Subsystem
- **Counters:** CD4518 (Dual BCD Counter)
- **Display Drivers:** CD4543 (BCD-to-7-Segment)
- **Logic:** CD4081 AND gates
- Counts from **00 to 59**, then resets and generates a carry signal to the next stage

### Hours Subsystem (24-Hour Format)
- **Counters:** CD4510 (BCD Up/Down Counter)
- **Display Drivers:** CD4543
- Counts from **00 to 23**, then resets to 00
- Incremented by the carry-out from the minutes counter

### Clock Source
- External **function generator**
- Square wave, **1 Hz frequency**
- Logic-level voltage compatible with CMOS ICs

---

## Key Components
- CD4518 – Dual BCD Counter  
- CD4510 – BCD Up/Down Counter  
- CD4543 – BCD-to-7-Segment Display Driver  
- CD4081 – Quad AND Gate  
- Seven-segment displays  
- Function generator  
- Oscilloscope and multimeter  
- Breadboard and discrete wiring  

---

## Implementation Highlights
- Each digit is driven by an independent BCD counter and display driver  
- Counters are cascaded using carry-out logic  
- AND-gate logic detects invalid count states and triggers resets  
- Entire system operates using **pure hardware logic**, reinforcing core digital design principles  

---

## Results
- Seconds and minutes counters operated correctly from **00–59**  
- Display updates were synchronized with the 1 Hz clock input  
- Carry logic successfully incremented higher-order counters  
- Minor instability was observed in the hours subsystem due to breadboard wiring limitations, which was documented and analyzed  

---

## Challenges and Lessons Learned
- Breadboard wiring density can introduce noise and intermittent behavior  
- Cascaded counters require careful signal timing and clean clock inputs  
- Incremental testing is critical when debugging multi-stage digital systems  

---

## Documentation
- Full lab report (PDF)
- Circuit schematics
- Photographs of the assembled circuit
- Demonstration videos showing clock operation

---

## Skills Demonstrated
- Digital logic design  
- Sequential circuits and counters  
- BCD encoding and decoding  
- Seven-segment display interfacing  
- Clock generation and synchronization  
- Hardware debugging and validation  

---

## Notes
This project was completed as part of an academic laboratory course and demonstrates hands-on experience with real hardware digital systems rather than simulation-only designs.
