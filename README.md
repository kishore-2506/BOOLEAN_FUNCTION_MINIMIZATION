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

Developed by: KISHORE M.

RegisterNumber: 212223040100

```
module ex02(A,B,C,D,F1);
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

**RTL realization**

**Output:**

![image](https://github.com/kishore-2506/BOOLEAN_FUNCTION_MINIMIZATION/assets/165657398/43b1db62-5af8-4d0c-ae87-98d79455c17f)

**RTL**

![image](https://github.com/kishore-2506/BOOLEAN_FUNCTION_MINIMIZATION/assets/165657398/f4f31e64-50ad-4c58-9743-14a6781546ef)

**Timing Diagram**

![image](https://github.com/kishore-2506/BOOLEAN_FUNCTION_MINIMIZATION/assets/165657398/779af228-1471-48c4-aedc-13fb93ce3f73)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

