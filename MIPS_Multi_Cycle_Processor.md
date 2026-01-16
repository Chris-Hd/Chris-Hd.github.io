# Multi-Cycle MIPS Processor (VHDL)  
**Computer Architecture & Structure Project**

## Overview  
This project focused on understanding the internal components and architecture of a multi-cycle MIPS processor by implementing and simulating it in VHDL. The processor was verified through simulation and tested using compiled machine code generated from MIPS assembly.

## Goal  
- Implement a multi-cycle MIPS processor in VHDL  
- Simulate and validate its behavior using ModelSim  
- Strengthen understanding of processor datapath, control, and multi-cycle execution

## My Role  
This was a team project. My main contributions were:
- Designed and implemented the **ALU** module  
- Built the **top-level integration** (connecting and integrating processor components)  
- Created the **testbench** to validate correct functionality and behavior

## Technologies Used  

**Tools**
- ModelSim (VHDL simulation)  
- MIPS compiler / assembler (assembly → machine code)

**Programming Languages**
- VHDL  
- MIPS Assembly

## What Worked Well  
- Successfully simulated processor execution in ModelSim  
- Verified functionality using testbench-driven validation and machine code test cases

## Challenges  
- Integrating the full processor at the top level (datapath + control)  
- Debugging and validating correct execution across the full instruction flow and timing
