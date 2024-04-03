# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

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

Developed by:KANAGAVEL.R

RegisterNumber:212223040085


**RTL realization**

![Screenshot 2024-04-03 100249](https://github.com/kanagavel7/BOOLEAN_FUNCTION_MINIMIZATION/assets/162578954/56d96b82-eb0b-42f1-b69a-b1442466cad1)

**Truth Table**

![Screenshot 2024-04-03 100333](https://github.com/kanagavel7/BOOLEAN_FUNCTION_MINIMIZATION/assets/162578954/6db05978-f04a-4d52-9614-bf89689e2cf0)

**Timing Diagram**

![Screenshot 2024-04-03 100402](https://github.com/kanagavel7/BOOLEAN_FUNCTION_MINIMIZATION/assets/162578954/f28c28bd-213d-4175-8efb-29263e409f0e)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

