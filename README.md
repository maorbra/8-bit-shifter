
**An 8-bit cyclic shifter** - A register that takes an input of 8 bits and shifts them according to another 3 bits input (for 8 bits shifter you have 8 options to shift the input between 0 to 7 shifts and to represent 8 options we need 3 bits). This chip is a small part of a computer structure with many registers.
 
The 8-bit shifter consists of 24 Mux_1_2 components.  Each mux gets 2 different input bits (A and B) and according to a selection bit input (S), outputs one of the inputs.

You can see here the schematic, the symbol, and the silicon layout design of the mux component. Using the CMOS method (the size of the transistors was computed according to the worst case of resistance).

You can see here the schematic, the symbol, and the silicon layout design of the 8-bit shifter made by the 24 muxes (3 rowes of 8) and 3 inverters(NOT gate). The first row takes every bit of the shifter input and according to the MSB of the 3 bit input, shifts(or not) the 8 bit input by 4. The second row takes the output from the first row, and according to the middle bit of the 3 bit input shifts(or not) the 8 bit input by 2. The third row takes the output from the second row, and according to the LSB of the 3 bit input shifts(or not) the 8 bit input by 1.

The concatenation of the 3 rows creates 8 bit shifter according to 3 bit input.

Example: 8-bit input: 00001111 ; 3-bit input: 011 - (3 shifts) ; output: 11100001

 
 
