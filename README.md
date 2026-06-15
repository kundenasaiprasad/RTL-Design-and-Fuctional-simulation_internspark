This project is an 8-bit ALU designed in Verilog and tested using a simple testbench.
Features
Addition
Subtraction
AND operation
OR operation
Inputs and Output
A[7:0] = first input
B[7:0] = second input
sel[1:0] = select signal
Y[7:0] = output
Operation
sel = 00 → Y = A + B
sel = 01 → Y = A - B
sel = 10 → Y = A & B
sel = 11 → Y = A | B
Testbench
The testbench applies different values of sel to check all ALU operations. It also creates a VCD file for waveform viewing in GTKWave. The common VCD workflow is to dump signals in the testbench and open the generated file in GTKWave �.
Simulation
To simulate:
Compile the design and testbench.
Run the simulation.
Open the waveform file in GTKWave.
Check that the output matches the selected operation �.
Result
The ALU works as a combinational circuit using an always @(*) block and case statement, which is a standard way to write simple ALU logic in Verilog
