# CPU Design on FPGA

A simple CPU datapath designed in VHDL and implemented on a Cyclone II FPGA using Quartus II. This project demonstrates core digital design concepts including FSMs, ALUs, decoders, latches, and 7-segment displays.

## Features
- 8-bit ALU with arithmetic and logical operations
- FSM-controlled opcode sequencing
- 3-to-8 decoder for ALU operation selection
- Dual 8-bit latches for operand storage
- Real-time output on 7-segment displays
- Waveform simulation and FPGA verification
- Multiple custom ALU variants

## Hardware / Tools
- Cyclone II FPGA (EP2C35F672C6)
- Quartus II
- VHDL
- Quartus Waveform Simulator

## CPU Components
- **FSM:** Controls operation sequencing through 8 states
- **Decoder:** Converts FSM states into one-hot ALU opcodes
- **Latches:** Store 8-bit operands A and B
- **ALU:** Performs arithmetic and logic operations
- **SSEG Driver:** Displays outputs and sign indicators

## ALU Variants

### ALU_1
- ADD, SUB, AND, OR, XOR, NAND, NOR, NOT

### ALU_2
Custom functions including:
- Increment
- Shift
- Rotate
- Min(A,B)
- Bit reversal
- XOR
- (A + B) - 4

### ALU_3
- Displays `y` if FSM student ID digit is odd
- Displays `n` if the digit is even

## Verification
Validated using:
- Waveform simulation
- Functional FPGA testing
- Real-time 7-segment display outputs

## Concepts Demonstrated
- RTL Design
- FSM Design
- Sequential Logic
- Opcode-Based Control
- FPGA Design Flow
- Hardware Verification

## Author
Ahmad Bhutta  
Computer Engineering Student  
Toronto Metropolitan University
