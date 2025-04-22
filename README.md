# 🕒 FPGA Digital Clock

A simple yet functional **Digital Clock** implemented on an **FPGA** using VHDL/Verilog. This project demonstrates real-time clock functionality with hours, minutes, and seconds, displayed using either a 7-segment display or VGA output (depending on configuration).

---

## 📦 Features

- ⏱️ 24-hour format timekeeping
- ⏳ Real-time seconds, minutes, and hour counting
- ⬆️ Manual time adjustment (optional buttons/switches)
- 🖥️ Display via:
  - 7-segment displays (HH:MM:SS)
  - Or VGA output (if supported)
- 🔄 Synchronous reset and clock divider for 1Hz timing

---

## 🧰 Tools & Requirements

- **HDL Language:** VHDL / Verilog (select based on your implementation)
- **Target FPGA Board:** [e.g., Xilinx Spartan-6 / Intel DE10-Lite / Basys 3]
- **Software Tools:**
  - [Xilinx Vivado / Intel Quartus Prime]
  - ModelSim / Vivado Simulator
- **Optional:** Push-buttons or DIP switches for manual time input

---

## 🗂️ Project Structure

```bash
fpga-digital-clock/
├── src/                # HDL source files
│   ├── clock_divider.v
│   ├── counter.v
│   ├── time_display.v
│   └── top_module.v
├── simulation/         # Testbenches
├── constraints/        # Pin constraints for FPGA board
├── docs/               # Block diagram, design notes
└── README.md
