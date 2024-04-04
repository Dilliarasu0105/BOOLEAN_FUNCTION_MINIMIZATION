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

Developed by:DILLIARASU M
RegisterNumber:212223230049

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
![image](https://github.com/Dilliarasu0105/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979593/15ac609c-5b02-4a2f-80a8-be43139f41db)

**RTL realization**
**Output:**
**RTL**
![image](https://github.com/Dilliarasu0105/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979593/7e3362e3-ac0b-4fd1-a1c6-3fad85e1a7ca)

**Timing Diagram**
![image](https://github.com/Dilliarasu0105/BOOLEAN_FUNCTION_MINIMIZATION/assets/144979593/57adb0e2-cfd3-485d-b024-7b084784a4ed)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

