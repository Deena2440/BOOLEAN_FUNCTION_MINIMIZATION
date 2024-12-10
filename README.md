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
```
module experiment2(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module experiment2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by: K.DEENATHAYALAN  RegisterNumber:24900766*/


**RTL realization**


![EXP-2  1](https://github.com/user-attachments/assets/0f8106d1-0c40-46b9-b88c-061090e65a3a)

![EXP-2 2](https://github.com/user-attachments/assets/5e8d9f77-d444-4cfd-8b95-a750cf97dc9f)

**Timing Diagram**
![EXP-2 waveform 1](https://github.com/user-attachments/assets/2a253aa3-b019-45a7-b653-6f7a53b30c68)

![exp-2 wave 2](https://github.com/user-attachments/assets/2fb036b0-8da9-4597-9574-1817378186a8)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

