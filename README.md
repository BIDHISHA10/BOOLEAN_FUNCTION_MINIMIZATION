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

Developed by: GOGINENI BIDHISHA
Register Number:212223040048*/


**RTL realization**
![WhatsApp Image 2024-04-04 at 15 08 21_610d87be](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/62a512c0-ab21-45e7-bca0-2c85bddfdf78)
![WhatsApp Image 2024-04-04 at 15 08 21_f8bc520a](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/a928d7ff-862a-4911-bba3-a3160bd1724a)

**Output:**
![WhatsApp Image 2024-04-04 at 15 08 21_4cbe0887](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/24702e7b-fae2-4d2c-82fb-9404b8635bdc)
![WhatsApp Image 2024-04-04 at 15 08 21_3afd60ca](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/7e1882be-991a-4555-94b9-092d5775251a)

**Timing Diagram**
![WhatsApp Image 2024-04-04 at 15 08 21_02102eb1](https://github.com/naavaneetha/BOOLEAN_FUNCTION_MINIMIZATION/assets/152273292/fa1f6b2b-687b-424a-9164-d619e9ea606e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

