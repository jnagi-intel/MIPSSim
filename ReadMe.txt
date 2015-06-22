Group 
Jaskaran Singh Nagi, UFID: 0119 0641, Email: jnagi@ufl.edu 
Satykrishna Kondapalli, UFID: 1553 4501, Email: satykrishna@ufl.edu

Follow the following steps to compile the code 
1. Untar the zip file 
	tar -zxvf MIPSSim.tar.gz 

2. Open the folder 
	cd MIPSSim/

   This folder should have the following files 
	MIPSSim.c
	MIPSSim.h
	DecodeInst.c
	FileHandling.c
	InstParser.h
	FuncProto.h
	fibonacci_bin.bin
	SimTomasulo.c
	SimTomasulo.h
	ListHandling.c
	btb.h
	btb.c
	makefile 
	

3. Build the project 
	make all 

4. Run the Simulation on fibonacci file
	To get the full output 
	./MIPSSim fibonacci_bin.bin fibonacci_out.txt 

	To get the final stage only 
	./MIPSSim fibonacci_bin.bin fibonacci_out.txt -T0:0

	To get cycles 15 to 20
	./MIPSSim fibonacci_bin.bin fibonacci_out.txt -T15:20

Note: 
For Branch and Jump Instructions, PC updated at the EX stage alongwith cancelling
of instructions fetched in ROB and RS after Branch/Jump. 

"On my honor, I have neither given nor received unauthorized aid on this assignment"