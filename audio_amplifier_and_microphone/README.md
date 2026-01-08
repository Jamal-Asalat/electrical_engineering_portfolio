# Audio Amplifier and Microphone System

## Overview
This project involves the design, simulation, construction, and testing of an audio amplification system capable of driving an 8 Ω speaker load. The system was developed as part of Electrical Engineering Laboratory II and focuses on practical amplifier design considerations such as efficiency, distortion, gain, biasing, and thermal stability.

The final implementation uses a **Class-B push-pull power amplifier topology**, selected after evaluating multiple amplifier configurations for performance and efficiency.

---

## Project Objectives
- Design an audio power amplifier capable of delivering **≥ 0.7 W** to an 8 Ω speaker  
- Operate from a **12 V DC supply**
- Achieve **> 40% efficiency**
- Minimize crossover distortion
- Maintain sufficient input impedance for audio signal sources
- Validate performance through simulation and physical measurements

---

## Design Approach
Several amplifier topologies were evaluated using circuit simulation, including:
- Direct source drive
- Common-emitter amplifier
- Emitter follower
- Class-B push-pull amplifier

Based on comparative analysis, the **Class-B push-pull amplifier** was selected due to its superior efficiency and ability to meet power and distortion requirements.

Key design considerations included:
- Proper biasing to reduce crossover distortion
- Thermal stabilization using emitter resistors
- Bias voltage generation using diode-connected transistors
- Optimization of efficiency and output swing

---

## Circuit Description
The final amplifier consists of:
- Complementary push-pull output transistors
- Capacitive coupling for AC signal transfer
- Emitter resistors for thermal stability
- Bias network to maintain approximately **0.6 V** base-emitter bias
- Load resistance of **8 Ω** representing a speaker

The amplifier was designed to operate at **1 kHz** with a sinusoidal input signal.

---

## Tools and Equipment
- Circuit simulation software (SPICE-based)
- Oscilloscope
- Function generator
- Multimeter
- DC power supply
- Discrete transistors, resistors, capacitors
- Protoboard for physical construction

---

## Performance Results
- **Output Power:** ≈ **1 W** into 8 Ω  
- **Efficiency:** ≈ **52%**  
- **Voltage Gain:** ~0.88 V/V  
- **Input Impedance:** ≈ **5.9 kΩ**  
- **Distortion:** Minimal, no observable crossover distortion  
- **Operation:** Stable across temperature variations

Measured experimental results closely matched simulated values, with small deviations attributed to component tolerances and wiring effects.

---

## Validation and Testing
- Transient simulations verified clean output waveforms without clipping
- DC operating point analysis confirmed proper biasing
- Oscilloscope measurements validated gain, output power, and efficiency
- Physical protoboard implementation demonstrated reliable real-world operation

---

## Documentation
- Full laboratory reports (PDF)
- Circuit schematics
- Simulation plots
- Measured oscilloscope waveforms
- Demonstration video of constructed amplifier (external)

---

## Key Skills Demonstrated
- Analog circuit design
- Audio power amplification
- Efficiency and thermal analysis
- SPICE simulation and verification
- Hands-on prototyping and measurement
- Interpretation of electrical schematics
