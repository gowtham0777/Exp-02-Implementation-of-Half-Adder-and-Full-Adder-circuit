NAME:GOWTHAM ADITYA R<br>
REFERENCE NUMBER:212223050018

# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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

![image](https://github.com/gowtham0777/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152005396/2e2b2d70-6cd9-44e5-995c-5ddfe453890d)

#### Figure -01 HALF ADDER 

![image](https://github.com/gowtham0777/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152005396/51a64acf-51e7-45b1-bd53-3dab07b90797)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows. 

Program:
# Half Adder:


module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule



# Full Adder


module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule



### TRUTH TABLE 
Half Adder Circuit:

![image](https://github.com/gowtham0777/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152005396/c5adea7a-d65a-4915-9aa3-3e570b1b0092)

Full Adder Circuit:-

![image](https://github.com/gowtham0777/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152005396/da436396-ccd5-4e92-9dc2-0409aca2edb6)

### RTL
Half Adder Circuit:

![image](https://github.com/gowtham0777/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152005396/cb7497f2-cd09-4be8-b5c1-0e24e6b7f3f4)

Full Adder Circuit:-

![image](https://github.com/Srikaran077/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/151993143/7e5d8d1d-f3c2-4f9a-a3cb-871f6d97443b)

### Output:
Half Adder Circuit:-

![image](https://github.com/gowtham0777/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152005396/216d5d27-8c80-4e2d-a425-9417f61cc752)

Full Adder Circuit:-

![image](https://github.com/gowtham0777/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152005396/6e60c24e-756f-4a05-ae3c-15ca70c8eace)

### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
