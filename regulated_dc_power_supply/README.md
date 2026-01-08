# Regulated DC Power Supply

## Overview
This project focuses on the design and analysis of a regulated DC power supply capable of delivering a stable output voltage under varying load conditions. The system was designed and evaluated using circuit simulation and measurement techniques to demonstrate effective voltage regulation and ripple reduction.

An unregulated rectifier and filter stage was first analyzed to highlight voltage drop and ripple behavior under load. A regulated supply was then implemented using a Zener diode reference and an op-amp–based voltage regulator to significantly improve load regulation and output stability.

## Objectives
- Design an unregulated AC-to-DC power supply using a transformer, bridge rectifier, and filter capacitor  
- Implement a regulated DC supply using a Zener reference and op-amp feedback  
- Achieve regulated output voltages of **6 V and 12 V** up to **200 mA load current**  
- Analyze load regulation and ripple voltage under light and heavy loads  
- Compare unregulated and regulated performance  

## Circuit Description
The power supply consists of the following stages:
- Step-down transformer and bridge rectifier for AC-to-DC conversion  
- Capacitor-based filtering to reduce ripple  
- Zener diode reference for voltage stability  
- Op-amp regulator with feedback network for output control  

Resistor values in the feedback network were selected to set the desired output voltage while minimizing current draw and improving regulation performance.

## Analysis & Results
### Unregulated Supply
- Significant voltage drop observed as load current increased  
- Load regulation ≈ **19%** at 200 mA  
- Ripple voltage increased substantially under heavier loads  

### Regulated Supply
- Output voltage remained stable across load conditions  
- **Load regulation:**  
  - ~0.5% at 6 V  
  - ~0.75% at 12 V  
- Ripple voltage remained below **25 mV peak-to-peak**, meeting design criteria  

Oscilloscope measurements confirmed simulation results, showing stable DC output with minimal ripple.

## Tools & Equipment
- Multisim (circuit simulation)
- Oscilloscope
- Function generator / AC source
- Multimeter
- Discrete diodes, capacitors, resistors
- Operational amplifier

## Key Takeaways
- Demonstrated the importance of voltage regulation in power supply design  
- Applied feedback control concepts using op-amp regulation  
- Evaluated real-world performance metrics such as ripple and load regulation  
- Strengthened understanding of power electronics and analog circuit design  

## Documentation
- Full lab report (PDF)
- Circuit schematics
- Transient and ripple analysis plots
