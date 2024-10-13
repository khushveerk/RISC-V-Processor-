# RISC-V-Processor-

## vedio 9

Risk Processor Design (00:03 - 10:00)





Starting with the risk processor design using Verilog.






Modules include instruction memory, instruction fetch unit, control unit, and data path.



Data path consists of ALU, register file, and data memory.

Instruction Memory





Instructions discussed include Type I, Type S, Type B, Type U.






Instructions are framed in binary format.



Memory locations store different instruction types.

Instruction Fetch Unit





Fetches instructions from instruction memory using the program counter.






Program counter acts as a pointer for fetching instructions.



Instructions are passed to the control unit for analysis.

Control Unit





Analyzes instruction fields including opcode and function values.






Determines the type of instruction (e.g., R type, S type, B type).



The control unit is crucial for understanding the instruction type.

Data Part





Consists of ALU, register file, and data memory.






Register file includes multiple registers with specific sizes.



Each register contains default data after a reset condition.

ALU Operations





ALU performs operations (e.g., addition, subtraction) using data from registers.






Takes data from two registers for operations.



Stores the result back in a register.

Top Module





Top module has two inputs: clock and reset signal.






Clock and reset signals provided by the test bench.



Contains all discussed modules.

Instruction Fetch Unit Inputs





Inputs include clock, reset (active high), and immediate address.






Immediate address is a part of control signals.



Control signals include beq, bnq, BGE, BLT, and jump instructions.

Branch Instructions (10:03 - 20:01)





"In the case of Branch instructions, we will give one immediate value."






"The PC will be jumping right, PC plus immediate value."



"If it is equal to one, then this instruction fetch unit will come to know that a BEQ instruction has been activated."






"The program counter will increment accordingly."

Instruction Memory





"In this instruction memory, all the instructions will be stored."






"Total four locations will constitute one instruction."



"This particular design is byte addressable."






"For every byte, there is one address."

Instruction Fetch Unit





"This PC incrementing logic will be performed by the instruction fetch unit."






"The output of this instruction fetch unit is the PC."



"This immediate address will also be calculated from the top model."






"We will give it to the instruction fetch unit."

Assignment for Instruction Memory





"Can you code for this instruction memory?"






"Each location should be of specified bits."



"If reset is applied, all these locations should be filled with binary value."






"The output of this instruction memory should be an instruction.

Program Counter Logic (20:03 - 23:30)





Immediate address is for jump control signals.






Program counter (PC) is generated and stored.



Logic for incrementing PC is discussed.



Reset conditions for PC.






If reset is true, PC is set to zero.



If branch instructions are equal to zero, PC is incremented normally.

Instruction Handling





Jump instructions and immediate address.






Immediate address is included in the instruction.



PC is incremented with the immediate address.



Storing return address in jump instructions.






The initial value of PC is stored for return.



Current PC will hold its value if certain conditions are met.

Instruction Fetch Unit





Completion of the instruction fetch unit logic.






Code will be shared for further understanding.



Upcoming session will discuss instruction memory unit integration.
