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
