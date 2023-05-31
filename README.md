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
Developed by: 
RegisterNumber:212222050042
*/
```
module exp2a (a, b, c, d, f1, f2);
input a,b,c,d;
output fl, f20
wire adash, bdash, cdash, ddash, x, y, z,p,
not (adash, a);
not (bdash,b);
not (cdash, c);
not (ddash, d);
and (x, bdash, ddash);
and (y, adash,b,d);
and (z, a,b,cdash);
or (fl, x, y, z);
and (p, cdash, d);
and (q, a, c);
and (r,b,c);
or (f2, p, q, r);
endmodule
```





## RTL realization
![exp2a](https://github.com/Nikkesh-VJ/Experiment--02-Implementation-of-combinational-logic-/assets/130572280/7e92907f-e50a-4cff-a61b-db65cebe8487)


## Output:
## RTL
## Timing Diagram
![Screenshot_20230421_024510](https://github.com/Nikkesh-VJ/Experiment--02-Implementation-of-combinational-logic-/assets/130572280/3a2a94f6-ff4a-48d1-a14f-35eaa56dfbe9)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
