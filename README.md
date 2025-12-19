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

Developed by:N.lakshmi pranay
RegisterNumber:25017706
*/
```
module exp1 (a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
assign f1 = ~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;
assign f2 = x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;
endmodul
```

**RTL realization**

<img width="739" height="794" alt="Screenshot 2025-12-19 105138" src="https://github.com/user-attachments/assets/ec017624-fe1a-4d4c-bd5d-d2533b9d1d7b" />


**RTL**

<img width="824" height="412" alt="Screenshot 2025-12-19 104333" src="https://github.com/user-attachments/assets/a6c4ba60-b1df-4098-a520-6e4d8e59c868" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

