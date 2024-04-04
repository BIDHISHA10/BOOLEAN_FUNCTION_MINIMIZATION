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
```
Developed by:GOGINENI BIDHISHA
RegisterNumber:212223040048
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule
```
*/
**RTL realization**
![WhatsApp Image 2024-04-04 at 15 08 21_d8022385](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/6e23abbe-b75e-4f0e-84a2-59903455e9f2)
![WhatsApp Image 2024-04-04 at 15 08 21_f456533a](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/bc2a5241-6d58-469b-8a7f-0a71ce698dc9)

**Output:**
![WhatsApp Image 2024-04-04 at 15 08 21_0633d47e](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/db60a9d3-ba29-4894-a594-bb30277d719a)
![WhatsApp Image 2024-04-04 at 15 08 21_275b5592](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/7f6d109a-a99f-4bc4-a7c8-92876170ceac)

**RTL**

**Timing Diagram**
![WhatsApp Image 2024-04-04 at 15 08 21_c92b19c8](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/658bc127-3516-4715-9e7a-6288787383a3)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

