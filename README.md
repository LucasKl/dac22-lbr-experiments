# dac22-lbr-experiments
This repository contains the implementation of the experiments for the DAC 2022 Late Breaking Results paper "A Toolbox for Waveform Based RISC-V Processor Analysis".

## File Description

### riscv-lib.wal
The library code for analyzing RISC-V processors. This code is generic and only requires some processor-specific code to be ported to new processors.

### vexriscv.wal
Processor-specific code for the [VexRiscv](https://github.com/SpinalHDL/VexRiscv) processor.
Implements the *Instruction per Cycle* and *Pipeline Stall* analysis.

### ibex.wal
Processor-specific code for the [IBEX](https://github.com/lowRISC/ibex) processor.
Implements the *Instruction per Cycle* and *Pipeline Stall* analysis.

### picorv32.wal
Processor-specific code for the [PicoRV32](https://github.com/YosysHQ/picorv32) processor.
Only implements the *Instruction per Cycle* analysis since PicoRV32 is not pipelined.

### serv.wal
Processor-specific code for the [SERV](https://github.com/olofk/serv) processor.
Only implements the *Instruction per Cycle* analysis since SERV is not pipelined.
