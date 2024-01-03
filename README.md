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

## Program:
/*
module project_3(sum,carry,a,b); 
input a,b; 
output sum,carry; 
xor sum1(sum,a,b); 
and carry1(carry,a,b); 
endmodule
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: SUDARSHANA S
RegisterNumber: 21222305050054 
*/
L
RTL realization:
![image](https://github.com/sudarshana11/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155507129/8f0a68b1-0fb7-4288-a436-cedb0146c466)

# timing diagram
![image](https://github.com/sudarshana11/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155507129/52480af6-339d-4a09-b19a-172f304c6b4a)

# truth table;
![image](https://github.com/sudarshana11/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155507129/addcaf73-9d21-4c9b-8da6-37db9ddb79c7)
 
# full adder;
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

![image](https://github.com/sudarshana11/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155507129/21283d47-571f-402f-9b14-4417f7a4c444)


Figure -02 FULL ADDER
# Program
module project_3_2(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c;
endmodule
RTL Realization
image

# TIMING DIAGRAM
![image](https://github.com/sudarshana11/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155507129/03ea2b9c-05b6-4f09-a4a0-0af5c6e241ad)


# TRUTH TABLE
![image](https://github.com/sudarshana11/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/155507129/b015a464-547a-435b-9a9e-a041d7c8e72d)

### Result:
Thus the given logic functions are implemented and their operations are verified using verilog programming
