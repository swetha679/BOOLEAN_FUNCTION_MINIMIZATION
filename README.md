# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II, USB flasher

**Software – Quartus prime**

**Theory**

Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions
**Logic Diagram**

![TRUTH TABLE (1)](https://github.com/user-attachments/assets/7cb55cc2-3634-4317-ad56-197eeb3839b0)


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
f1
'''module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule '''

f2
'''
module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule '''







**RTL realization**

f1 

![Screenshot (46)](https://github.com/user-attachments/assets/7fcd5934-8fda-437f-b480-ff59b7be02a1)


f2


![Screenshot (48)](https://github.com/user-attachments/assets/6348c472-a0ca-48a6-9985-0fa995ebba9f)




**Output:**

f1

![Screenshot (104)](https://github.com/user-attachments/assets/23e04f42-33f9-4f78-8fbe-035f92e8979c)


f2

![Screenshot (105)](https://github.com/user-attachments/assets/dacc8f0c-f026-449f-82ee-7f35a42c6916)


**Result:**

Thus the given logic functions are implemented und their operations are verified using Verilog programming.

