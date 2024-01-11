# Simulator

<p>This Python code provides a simulator for a 16-bit ISA (Instruction Set Architecture) that supports various instructions and opcodes. The simulator allows you to execute binary instructions and observe the effects on the registers and flags.</p>

<h2>ISA Description</h2>

The ISA supports a 16-bit architecture with the following instructions and opcodes, along with their syntax:
- Addition (add reg1 reg2 reg3)
- Subtraction (sub reg1 reg2 reg3)
- Move Immediate (mov reg1 $Imm)
- Move Register (mov reg1 reg2)
- Load (ld reg1 mem_addr)
- Store (st reg1 mem_addr)
- Multiply (mul reg1 reg2 reg3)
- Divide (div reg3 reg4)
- Right Shift (rs reg1 $Imm)
- Left Shift (ls reg1 $Imm)
- Exclusive OR (xor reg1 reg2 reg3)
- OR (or reg1 reg2 reg3)
- AND (and reg1 reg2 reg3)
- Invert (not reg1 reg2)
- Compare (cmp reg1 reg2)
- Unconditional Jump (jmp mem_addr)
- Jump If Less Than (jlt mem_addr)
- Jump If Greater Than (jgt mem_addr)
- Jump If Equal (je mem_addr)
- Halt (hlt)
The ISA includes 7 general-purpose registers (R0 to R6) and 1 flag register (FLAGS). Each register is 16 bits in size.

<h2>Usage</h2>

To simulate the execution of binary instructions, follow these steps:

  1. Define the binary instructions in a list, where each element represents a 16-bit instruction.
     
  2. Create an instance of the BinaryInstructionSimulator class by passing the binary instructions list as an argument.
     
  3. Call the simulate() method on the simulator instance to execute the instructions.
   
  4. After simulation, you can access the current state of registers and flags using the registers and flags attributes of the simulator instance.

<h2>Simulate the execution of instructions</h2>
    
    1. python3 Simulator.py
    2. enter all the instructions line by line
    3. press Ctrl+Z to get the output

<h2>Example</h2>
Here's an example code snippet that demonstrates how to use the binary instruction simulator:

  Define the binary instructions
 
    0b0000000000101011,  # add R1, R2, R3
    0b0000100100101011,  # rs R2, $4
    0b0010000000110010,  # ld R0, 1100100
    0b1001000000000100   # jlt 00000100

