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
module exp2(a, b, c, d, w, x, y, z, f1, f2);

input a, b, c, d, w, x, y, z;
output f1, f2;

assign f1 = ((~b & ~d) | (~a & b & d) | (a & b & ~c));

assign f2 = ((~y & z) | (w & y) | (x & y));

endmodule
```

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:udhayamoorthy A RegisterNumber:212225040477


**RTL realization**

**Output:**
<img width="575" height="553" alt="596492575-ff6c788f-a7fe-4f7c-8a2f-ff18ba25dacf" src="https://github.com/user-attachments/assets/5954d18f-314d-4b90-9b6f-7ffad7da99d0" />


**RTL**
<img width="1920" height="1080" alt="597718719-61f93df7-8c7f-446c-ac83-327b654484d6" src="https://github.com/user-attachments/assets/5ca25b61-aad8-4b03-bc7e-ba9d60855af6" />


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

