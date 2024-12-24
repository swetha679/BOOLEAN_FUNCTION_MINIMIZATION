# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher


**Software – Quartus prime** 

**Theory**
Boolean Algebra is a branch of algebra that deals with boolean values—true and false. It is fundamental to digital logic design and computer science, providing a mathematical framework for describing logical operations and expressions

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
 

Developed by:
RegisterNumber:

module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~b & ~d)|(~a & b & d)|(a & b & ~c));
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((~y & z)|( w & y )|(x & y));
endmodule




**RTL realization**

![Screenshot (46)](https://github.com/user-attachments/assets/dcd59548-f2c5-4d06-b380-9b42cad00deb)


![Screenshot (48)](https://github.com/user-attachments/assets/09c4741b-7451-40cf-8482-8e1f4b35ad1b)



**Output:**

![Screenshot (104)](https://github.com/user-attachments/assets/01cfc80e-2166-44d1-bcc8-365025b6e749)


![Screenshot (105)](https://github.com/user-attachments/assets/961643a6-cb96-4220-b614-3552e9598d7b)




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

