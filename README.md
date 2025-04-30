# Verilog ALU

## 🧩 Overview

A simple ALU in Verilog supporting:
- Addition & Subtraction (18-bit ripple-carry adder)
- Multiplication (Booth algorithm)
- Division (Non-restoring method)

## ⚙️ Modules

- `alu.v` – Main ALU controller
- `adder.v` – 18-bit signed adder/subtractor
- `booth_multiplier.v` – 8-bit Booth multiplier
- `non_restoring_division.v` – 16-bit / 8-bit divider
- `fac.v` – Full adder used in the adder chain
- `control_unit.v` – Booth pattern decoder

## 🚀 Usage

Select operation with `op_select`:
- `00` → Add
- `01` → Subtract
- `10` → Multiply
- `11` → Divide

Outputs result on `res` and signals completion via `done`.

---