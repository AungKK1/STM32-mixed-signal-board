# STM32 Mixed-Signal Embedded Board
This project is a 4-layer mixed-signal embedded hardware system designed with Altium Designer. It integrates STM32F407 with Ethernet, USB, motor control, and audio interfaces. The design emphasizes mixed-signal partitioning, power distribution, and thermal management.

---

## 🧠 Objective

To design a complex mixed-signal PCB using STM32F407 and supporting peripherals for embedded applications, while applying best practices in signal integrity, grounding, and PDN analysis.

---

## ⚙️ Core Components

- **STM32F407VGT6** – High-performance ARM Cortex-M4 microcontroller
- **STM32F103** – Used as a debugger
- **DP838261ERHBR** – Ethernet PHY
- **DRV8701E** – Dual H-Bridge motor driver
- **CH340C** – USB-to-Serial bridge
- **ADS122C04** – 24-bit delta-sigma ADC
- **Stereo DAC** + audio codec + MIC
- **Linear regulators**, power switches, level shifters

---

## 🔌 Interfaces

- **USB** (Firmware upload & debug)
- **Ethernet** (Network control & communication)
- **I²C / SPI / UART** – Peripheral and sensor interfaces
- **Audio** – DAC output, MIC input, codec for stereo processing
- **Motor Control** – 2-channel motor driver interface

---

## 💡 Design Highlights

- **4-layer PCB stack-up** optimized for signal/power integrity
- Careful **ground-split strategy** between analog and digital domains
- **PDN analysis** using Altium PDN Analyzer
- **24-bit ADC** layout with low-noise analog front-end
- **Audio routing** with impedance-matched traces and filtering
- **Motor driver** with MOSFET H-bridge, heat dissipation plan
- **Differential pairs** for Ethernet and USB
- **EMC mitigation** using planes, shielding, and RC filters

---

## 📎 Files

- [`/docs`](./docs): Schematics, layout images, stackup, PDN snapshots
- [`/gerbers`](./gerbers): Fabrication-ready files
- [`/odb++`](./odb++): Full manufacturing format
- [`/bom`](./bom): Bill of Materials
- [`/simulation`](./simulation): PDN or thermal analysis (if available)

---

## 👨‍🏫 Acknowledgments

This project is based on **Aviral Mishra's Complete Hardware Design Course** and refined through Altium Designer simulations and reference materials.

---

## 🚫 Disclaimer

This board has not yet been prototyped. It was designed for educational purposes to demonstrate system-level embedded hardware design.
