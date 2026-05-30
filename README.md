# Power Electronics Simulation Tools

MATLAB/Simulink and LTSpice simulation projects from the *Power Electronics* laboratory course at AGH University of Science and Technology (Kraków), Electrical Engineering.

## Projects

### 1. Three-Phase Thyristor Bridge Rectifier
`Simulink/ThreePhaseInverter/` — Jakub Cios, Maciej Duda (Nov 2023)

Six-thyristor bridge converting three-phase AC to DC. Analysis performed in MATLAB Simulink:
- Effect of firing angle ALFA (0°–135°) on: phase current waveforms, active/reactive/apparent power (P/Q/S), power quality parameters (THD, cos φ), average DC output voltage U_dc
- Effect of input inductance L_in on: input current waveform, FFT harmonic spectrum, average U_dc
- Effect of network equivalent reactance on input voltage distortion

![Three-phase thyristor bridge model](https://github.com/JackobPunch/PowerElectronicsSimulationTools/blob/main/Simulink/ThreePhaseInverter/image.jpg)

---

### 2. Single-Phase Inverters
`Simulink/OnePhaseInverters/` — Jakub Cios (Dec 2023)

Two inverter topologies simulated in MATLAB Simulink:
- **Half-bridge inverter** — switching signals, dead time analysis, output voltage and current waveforms under varying load resistance
- **Full-bridge inverter with bipolar sinusoidal PWM** — modulation depth coefficient m_a effect on output RMS voltage, dead time effect on output waveform quality, output current ripple measurement and calculation

![Single-phase inverter waveforms](https://github.com/JackobPunch/PowerElectronicsSimulationTools/blob/main/Simulink/OnePhaseInverters/PrzebiegiModel3.jpg)
![Single-phase inverter waveforms 2](https://github.com/JackobPunch/PowerElectronicsSimulationTools/blob/main/Simulink/OnePhaseInverters/PrzebiegiModel3_2.jpg)

---

### 3. Fullbridge Push-Pull Converter (Switching Power Supply)
`LTSPice/FullbridgePush-PullConverter/` — Jakub Cios (Mar 2024)

High-frequency switching power supply with full-bridge inverter and HF transformer simulated in LTSpice:
- **Topology:** 230V AC input → bridge rectifier → full-bridge MOSFET inverter (IRF6644) → HF transformer → output rectifier + LC filter
- **PWM control:** UC3525 IC — duty cycle regulation, dead time, soft start
- **Characteristics:** output voltage vs. t_on time (linear, 5–20 µs → 16.6–55.9 V), output voltage vs. load current (drooping characteristic under overload)

![LTSpice model](https://github.com/JackobPunch/PowerElectronicsSimulationTools/blob/main/LTSPice/FullbridgePush-PullConverter/model.png)
![Waveforms](https://github.com/JackobPunch/PowerElectronicsSimulationTools/blob/main/LTSPice/FullbridgePush-PullConverter/Przebiegi.jpg)

## Authors

Jakub Cios — Electrical Engineering, AGH University of Science and Technology, Kraków
Maciej Duda (Three-Phase Thyristor Bridge only)
