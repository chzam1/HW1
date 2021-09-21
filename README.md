# HW1

Repository in github refers to a directory or storage space where your projects can live. This repository covers seven examples of Hardware Description Language (HDL). The examples covered are based on SystemVerilog (SV) HDL. Futhermore, all the examples were recreated using python and used to reference the behavior of the SV code. Testbench was used to test the files written in SystemVerilog which is required to run a simulation. Cocotb which is a python library was used to create the testbenches in this repository. 

# Examples covered:
  1. Combinational Logic
  2. Logic Gates
  3. Full Adder
  4. Register
  5. Resettable Register:
      1. Synchronous
      2. Asynchronous
  7. Full Adder (Using Nonblocking Assignments)
  8. History FSM (Finite State Machine)

# An Introduction to SystemVerilog
## 1) Modules:
A module is a block of Verilog code that implements a certain functionality. Modules can be embedded within other modules and a higher level module can communicate with its lower level modules using their input and output ports.

1. Behavioral Modules:
Behavioral models in Verilog contain procedural statements, which control the simulation and manipulate variables of the data types. These all statements are contained within the procedures. The initial statement is then completed and is not executed again during that simulation run. It is also a description in Verilog is used to describe the function of a design in an algorithmic manner.

2. Structural modules:
Structural Verilog is usually referred to a Verilog code which is synthesizable (has an accurate and meaningful hardware realization) and is usually written in Register Transfer Level (RTL).

## 2) Precedence operators:
Operator precedence determines how operators are parsed concerning each other. Operators with higher precedence become the operands of operators with lower precedence.

## 3) Numbers:
You can specify constant numbers in decimal, hexadecimal, octal, or binary format. Negative numbers are represented in 2's complement form. When used in a number, the question mark (?) character is the Verilog alternative for the z character.

## 4) Zs and Xs (signal values):
Hardware description languages such as SystemVerilog use the symbol ‘X’ to describe any unknown logic value. If a simulator is unable to decide whether a logic value should be a ‘1’, ‘0’, or ‘Z’ for high impedance, it will assign an X. In simulation, High-Z can be either an acceptable state (e.g. if you are observing a tristate I/O pin), or an indicator of a major problem (e.g. if you use a generate loop and miss a bit in a data bus it will go High-Z).

## 5) Testbench
A testbench is simply a Verilog module. But it is different from the Verilog code we write for a DUT. Since the DUT's Verilog code is what we use for planning our hardware, it must be synthesizable. Whereas, a testbench module need not be synthesizable. We just need to simulate it to check the functionality of our DUT

# Testbench with cocotb
cocotb is a COroutine based COsimulation TestBench environment for verifying VHDL and SystemVerilog RTL using Python. Cocotb is completely free, open source (under the BSD License) and hosted on GitHub. Cocotb requires a simulator to simulate the HDL design and has been used with a variety of simulators on Linux, Windows and macOS. A (possibly older) version of cocotb can be used live in a web browser on EDA Playground.



# References
-cocotb’s documentation!  
-HDL Introduction pdf  
-Google
