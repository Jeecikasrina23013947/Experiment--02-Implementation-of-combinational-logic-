# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: JEECIKASRINA M 
RegisterNumber:23013947  


##  CODE:
module verilog1(a,b,c,d,w,x,y,z,F1,F2);
input a,b,c,d,w,x,y,z;
output F1,F2;
wire  A1,A2,A3,A4,A5,B1,B2,B3,B4,B5;
assign A1= (~a&(~b)&(~c)&(~d));
assign A2= (a&c&(~d));
assign A3= ((~b)&c&(~d));
assign A4= (~a&b&c&d);
assign A5= (b&(~c)&d);
assign F1= A1|A2|A3|A4|A5;
assign B1= (x&(~y)&z);
assign B2= (~x&(~y)&z);
assign B3= (~w&x&y);
assign B4= (w&(~x)&y);
assign B5= (w&y&z);
assign F2= B1|B2|B3|B4|B5;
endmodule


##  TRUTH TABLE:

![image](https://github.com/Jeecikasrina23013947/Experiment--02-Implementation-of-combinational-logic-/assets/148515300/b9975783-14f7-4f67-8c32-4a09e3b8c82f)


##RTL VIEW:

![image](https://github.com/Jeecikasrina23013947/Experiment--02-Implementation-of-combinational-logic-/assets/148515300/70cf4e8f-9c2e-435b-896d-5e92d7ea9a57)


##OUTPUT:

![image](https://github.com/Jeecikasrina23013947/Experiment--02-Implementation-of-combinational-logic-/assets/148515300/72a9eb7f-cb29-42b6-b3c0-4cc0d4f1563f)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
