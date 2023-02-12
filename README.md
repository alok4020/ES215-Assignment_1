# ES215-Assignment_1
R-type triadic instructions of SDLX processor implementation on basys3 board.
To implement R-type triadic instruction to perform following operations:
	(ADD, SUB, AND, OR, XOR, SLL (shift left logical), SRL (shift right logical), SRA (shift right arithmetic), ROL (rotate left), ROR (rotate right), SLT (signed less than comparison), SGT (signed greater than), SLE (signed less than or equal to comparison), SGE, UGT, ULT, ULE, UGE.

Set the switches to IR7:0 .
Give a clk through push button p1.
Set the switches to IR15:8
Give a clk through push button p2.
Set the switches to IR23:16 .
Give a clk through push button p3.
Set the switches to IR31:24 .
Give a clk through push button p4.
Processor clk through P5
See the output of ALU on LED.


Solution:------------------------------------------------------------------------------------------------------------------------------------------------------
Assumptions: 
Initially, we have initialised the data in memory  [31:0]RegFile[31:0] using the initial block. 
Each location contains the square value corresponding to the location. 
1st  location contains 1, 2nd location contains 4, similarly, ith location contains i*i value as shown in Figure 1 below.
For eg. if RS1=1; D1_OUT = 1, RS1 = 2; D1_OUT = 4, and so on.
We are aware of the fact that  the SDLX doesn’t have any multiplier block. We have just used the initial block for initialisation. We could have used any other initialisation pattern.
LSB is an extra variable, which we have taken in order to show our 32 bit outputs using 16 LEDs available. When LSB=1, then LEDs show lower 16 bits and when LSB=0, then LEDs show upper 16 bits.




