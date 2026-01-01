# ECE259-Labs
Assembly / System Verilog code, with applications on an FPGA

## Lab2
Implementation of digital logic circuits using SystemVerilog. This lab focuses on hierarchy, module instantiation, and designing 2-to-1 and 7-to-1 multiplexers verified through ModelSim simulations.


## Lab3
Design and implementation of a 4-bit Ripple Carry Adder and an Arithmetic Logic Unit (ALU). This project explores hierarchical design, combinational logic for arithmetic operations, and sequential logic using D-flip-flops and registers.


## Lab4
Implementation of advanced sequential logic in SystemVerilog. This project features a 4-bit rotating register with arithmetic shift capabilities and a flexible rate-divided hexadecimal counter.


## Lab5
Implementation of Finite State Machines (FSMs) in SystemVerilog to control digital systems. This project features a pattern-recognizing FSM and a simple processor architecture with a defined control path and datapath.


## Lab6
Developing assembly language scripts for the DE1-SoC Computer System. Features implementations of integer list summation, item counting, and an efficient shift-and-AND algorithm to determine the longest consecutive string of ones in a 32-bit word.


## Lab7
An exploration of RISC-V assembly subroutines and calling conventions. Includes a recursive bit-counting algorithm and an in-place Bubble Sort implementation for 32-bit unsigned numbers. Uses a subroutine ONES that counts the longest string of consecutive 1s in a list of words. Adherence to "caller-saved" (t0–t6) and "callee-saved" (s0–s11) register rules3.


## Lab8
Interfacing RISC-V assembly with DE1-SoC hardware peripherals. Features binary counter control via pushbutton polling and precision timing using hardware interval timers. Using base addresses like 0xFF200000 (LEDs) and 0xFF200050 (Pushbuttons) to control external hardware. Handling asynchronous user input by reading and resetting the Edge-capture register. Configuring a 100 MHz interval timer to generate a precise 0.25-second delay instead of using software delay loops.


## Lab9
Advanced RISC-V assembly implementing an interrupt-driven system for a hardware counter. Demonstrates real-time responsiveness by handling asynchronous timer and pushbutton events via an interrupt handler. Setting up the mtvec (Machine Trap-Vector Base-Address) register and using mret (Machine Trap Return).

Interrupt Service Routines (ISRs): 
- Timer_ISR: Increments a global COUNT variable every 0.25 seconds.
- KEYS_ISR: Toggles the RUN state or modifies the timer's load value to double/halve the counting speed.
