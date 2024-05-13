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

Developed by:VIDHIYA LAKSHMI S
RegisterNumber:212223230238
```
module booleanfunction_top(a,b,c,d,w,x,y,z,f1,f2);
input a,b,c,d,w,x,y,z;
output f1,f2;
wire adash,bdash,cdash,ddash,ydash,p,q,r,s,t,u;
not(adash,a);
not(bdash,b);
not(cdash,c);
not(ddash,d);
not(ydash,y);
and(p,bdash,ddash);
and(q,adash,b,d);
and(r,a,b,cdash);
or(f1,p,q,r);
//type code for f2 as like f1
endmodule
```


**Program:**

![Screenshot (72)](https://github.com/saravidhya/BOOLEAN_FUNCTION_MINIMIZATION/assets/87062069/93fcddb0-68fb-42e8-b841-598dd7e45b88)



**RTL realization**

![Screenshot 2024-03-19 085049](https://github.com/saravidhya/BOOLEAN_FUNCTION_MINIMIZATION/assets/87062069/ed35ba9c-0c64-4591-b3c3-2c11da23e846)




**Output:**

![Screenshot (73)](https://github.com/saravidhya/BOOLEAN_FUNCTION_MINIMIZATION/assets/87062069/473d98e3-ebc3-4b46-979e-b89ab39372a2)



**Truth table**
![Screenshot 2024-03-21 090538](https://github.com/saravidhya/BOOLEAN_FUNCTION_MINIMIZATION/assets/87062069/70f06efb-69f7-4b40-89ff-8961d6234354)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

