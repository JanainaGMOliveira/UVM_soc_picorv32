# UVM Verification — SoC IoT PicoRV32 AXI

UVM testbench developed during the **CI Digital Program** to verify the [SoC IoT PicoRV32 AXI](https://github.com/danilolimadev/soc_iot_picorv32_axi) — a PicoRV32-based System-on-Chip with AXI4-Lite interconnect targeting IoT applications.

---

## Overview

This repository contains the **Universal Verification Methodology (UVM)** environment for functional verification of the SoC IoT PicoRV32 AXI. The DUT (Device Under Test) is the full SoC, including the PicoRV32 core, AXI4-Lite interconnect, peripherals (GPIO, UART, SPI, I2C, TIMER, RAM) and a bootloader.

---

## UVM Testbench Architecture
// TODO: divide files for each class

```
uvm_tb/
├── uvm_tb_top.sv
├── bfm.sv
├── soc_macros.svh
├── soc_pkg.sv
├── transaction.sv
├── tests/
│   └── soc_test.sv
├── env/
│   └── environment.sv
├── agents/
│   ├── agent.sv
│   ├── driver.sv
│   ├── monitor.sv
│   └── sequencer.sv
├── sequences/
│   ├── sequence.sv
├── scoreboard/
│   └── scoreboard.sv
└── coverage/
    └── coverage.sv
```

### Component Roles

TODO: add description of each component

---

## ✅ Verification Results

// TODO: add results and needed tests

| Test | Status | Notes |
|---|---|---|
| GPIO read | ✅ PASS | |
| UART TX sequence | ✅ PASS | |
| SPI | ✅ PASS | |
| I2C | ✅ PASS | |
| TIMER | ✅ PASS | |

---

## 🔗 Related Repository

The DUT (SoC source files) is maintained separately:  
👉 [soc_iot_picorv32_axi](https://github.com/danilolimadev/soc_iot_picorv32_axi)

---