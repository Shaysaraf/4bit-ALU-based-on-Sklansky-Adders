# 4bit-ALU-based-on-Sklansky-Adders
Verilog design for a 4bit ALU based on Sklansky Adders
Verilog design of a 4-bit Arithmetic Logic Unit (ALU) using Sklansky adders for operands represented in two's complement form. 
The ALU performs as following:
inputs: clk, [3:0] A, [3:0] B, [3:0] C.
outputs: [4:0] X, [5:0] Y.
functionality: X = A + B, Y = X - C

The ALU uses 2 main modules, one is a 4-bit adder without carry-in (for calculating X), and the other is a 5-bit
subtractor based on the two's comp. negative transformation of a string, -C = ~C + 1, and it has a constant carry-in of 1 (for calculating Y).
