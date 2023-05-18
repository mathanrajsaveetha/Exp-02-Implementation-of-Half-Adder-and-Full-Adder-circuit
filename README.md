# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:MATHAN RAJ 
RegisterNumber:  212222230079
```
###HALF ADDER
module half_adder(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule
###FULL ADDER
module full_adder (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule
```




### Output:

### HALF ADDER
![image](https://github.com/mathanrajsaveetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560501/305c3459-e0b8-444c-aad8-dd925aea04e8)
### FULL ADDER
![image](https://github.com/mathanrajsaveetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560501/fe0af859-e8ed-402f-b424-3f2d39d77e2c)


### RTL
### HALF ADDER
![image](https://github.com/mathanrajsaveetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560501/e240a9be-eba2-425a-9ef9-746f5108b4c4)
### FULL ADDER
![image](https://github.com/mathanrajsaveetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560501/5cde060c-32d0-4f36-94f5-63014ee97480)



### TIMING DIAGRAM
### HALF ADDER
![image](https://github.com/mathanrajsaveetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560501/5d9f395d-2904-43bc-bdba-3a3b6ae84e68)
### FULL ADDER
![image](https://github.com/mathanrajsaveetha/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560501/71ffdf84-bc36-4890-bc9c-bfc995cd121f)



### Result:
Thus,the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
