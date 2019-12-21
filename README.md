# MiniVm

This Virtual Machine is written en C. We made it as a final proyect for the Computer Architecture class.

## Summary

MiniVM is a reduced Virtual Machine that has his own memory and language for executing programs. This language has (initially) 17 instructions (NOP, MOV, LW, PUSH, POP, PRINT, READ, ADD, SUB, MUL, DIV, CMP, JMP, JMPE, JMPL and HLT), and works iwth 4 bytes operantors. 

To execute a code, you need to have a code in .asm, and simply use the terminal.

The MiniVM parse the code, using yyparse() and processLabels(), and converts it to an array of Instructions (the struct is in the code). Then prints it, and executes the run() function, that basically, runs instruction after instruction until it reachs a HTL.
