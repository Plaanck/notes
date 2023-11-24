



# Addressing Memory

- There are 4 main ways of addressing memory, to do with inspecting the opcode and operand

1) **Immediate Addressing**
	- Here, the operand is seen as actual data, meaning 1000 1111 (letting 1000 mean add) would translate to ADD 15, meaning the operand is the number that the operator will work on
	- This is quite useless though, as the maximum number you can use with an 8 bit instruction is 15, which isn't very useful

2) **Direct Addressing**
	- Here, the operand is the memory address that holds the value that will be worked on by the operator. E.G. 1000 1111 (Let's say that 00000001 is held in that address) that would translate to ADD 1
	- This is better, as it allows for more numbers to be utilised, at this point it is 15 numbers.

3) **Indirect Addressing**
	- Here, the operand points to a memory address, which points to another memory address, which holds the value to be worked on. E.G. 1000 1111 points to memory address 00001111, which could hold value 10101111, and if you go to memory address 10101111, the value held in there is the one that will be worked on.
	- This is even better, as it allows 8-bit memory addresses to be utilised, meaning 255 numbers can be used.