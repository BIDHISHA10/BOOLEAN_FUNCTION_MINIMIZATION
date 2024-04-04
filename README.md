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

Developed by:GOGINENI BIDHISHA 
RegisterNumber:212223040048
*/
```
module combinationalcircuit(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```
![image](https://github.com/BIDHISHA10/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/b593322a-7238-4de8-b39e-5ecaf51dea99)

**RTL realization**
![image](https://github.com/BIDHISHA10/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/90543809-eb4e-46af-a82c-025951e28495)

**Output:**
![image](https://github.com/BIDHISHA10/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/c8d18889-5e2d-4db1-8b1a-2dfdb61773f3)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

