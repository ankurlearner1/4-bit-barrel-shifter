# 4-bit-barrel-shifter
# 4-Bit Bidirectional Barrel Shifter

## 📌 Overview

This project implements a **4-bit bidirectional barrel shifter** using Verilog HDL.

A barrel shifter is a combinational digital circuit capable of shifting or rotating a binary data word by a specified number of positions without requiring multiple clock cycles.

This implementation supports:

- Left shifting
- Right shifting
- Shift amounts from 0 to 3 positions
- 4-bit input and output data
- Simulation using Icarus Verilog
- Waveform verification using a VCD file

---

## 🧩 Design Specification

| Parameter | Description |
|---|---|
| Data Width | 4 bits |
| Shift Control | 2 bits |
| Direction | 1 bit |
| Output | 4 bits |
| Shift Range | 0–3 positions |
| Design Type | Combinational |
| HDL | Verilog |
| Simulator | Icarus Verilog |

---

## ⚙️ Inputs and Outputs

| Signal | Width | Description |
|---|---:|---|
| `data_in` | 4 bits | Input data |
| `shift` | 2 bits | Number of positions to shift |
| `dir` | 1 bit | Direction control |
| `data_out` | 4 bits | Shifted output |

### Direction Control

| `dir` | Operation |
|---:|---|
| `0` | Left shift |
| `1` | Right shift |

### Shift Control

| `shift` | Shift Amount |
|---|---:|
| `00` | 0 |
| `01` | 1 |
| `10` | 2 |
| `11` | 3 |

---

## 🏗️ Block Diagram

```text
             ┌─────────────────────────┐
             │   4-Bit Barrel Shifter  │
             │                         │
data_in ────►│                         │────► data_out
             │                         │
shift ──────►│     Shift Control       │
             │                         │
dir ────────►│     Direction Control   │
             └─────────────────────────┘


🛠️ Tools Used
Verilog HDL
Icarus Verilog
VS Code
GitHub Codespaces
VCD waveform simulation



4-bit-barrel-shifter/
│
├── 4bitbarrelshifter.v
├── 4bitbarrelshifter_tb.v
├── README.md
├── LICENSE
└── .gitignore


👨‍💻 Author
Ankur Kumar
Electronics and Communication Engineering