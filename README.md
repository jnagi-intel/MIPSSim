# MIPSSim
MIPS32 Pipeline Simulation using Tomasulo Algorithm with out of order execution and in order commit along with a branch predictor using Branch Target Buffer

To get the full output 
	./MIPSSim fibonacci_bin.bin fibonacci_out.txt 

To get the final stage only 
	./MIPSSim fibonacci_bin.bin fibonacci_out.txt -T0:0

To get cycles 15 to 20
	./MIPSSim fibonacci_bin.bin fibonacci_out.txt -T15:20

Note: 
For Branch and Jump Instructions, PC updated at the EX stage alongwith cancelling
of instructions fetched in ROB and RS after Branch/Jump. 

