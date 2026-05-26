# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:KOPIGA N
RegisterNumber: 212225220053*/

```
module de2 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodule
```

**RTL realization**
**Output:**
<img width="513" height="502" alt="image" src="https://github.com/user-attachments/assets/59dd9e76-a44e-4470-be39-5efb224ec9be" />

**RTL**
**Timing Diagram**
<img width="823" height="407" alt="image" src="https://github.com/user-attachments/assets/54c6e606-7a32-4131-8f1b-f190fcc627d3" />

**Result:**
Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

