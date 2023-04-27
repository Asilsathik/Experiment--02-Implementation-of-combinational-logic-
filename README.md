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
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: MOHAMED ASIL
RegisterNumber:212222230080  
```
```
module tt1(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,Y,X,Z;
output F1,F2;
wire A1,A2,A3,A4,A5,B1,B2,B3,B4,B5;
assign A1 = ((~A)&(~B)&(~C)&(~D));
assign A2=(A&(~C)&(~D));
assign A3=((~B)&C&(~D));
assign A4=((~A)&B&C&D);
assign A5=(B&(~C)&D);
assign B1=(X&(~Y)&Z);
assign B2=((~X)&(~Y)&Z);
assign B3=((~W)&X&Y);
assign B4=(W&(~X)&Y);
assign B5=(W&X&Y);
assign F1=(A1|A2|A3|A4|A5);
assign F2=(B1|B2|B3|B4|B5);
endmodule
```
## Output:

## RTL realization:

![RTL2](https://user-images.githubusercontent.com/119476247/234773359-aa3416d9-a0d5-49a6-80dc-979cb1474e4f.png)
![RTL1](https://user-images.githubusercontent.com/119476247/234773404-a41f3489-a601-4da8-9864-d01a50ad7b72.png)

## Timing Diagram
![RTL](https://user-images.githubusercontent.com/119476247/234773735-0b9060e3-fdb0-4da1-92ea-de5041d9a4ed.png)

## RESULT :
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
