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

```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Bejin.B
RegisterNumber:22001908
Program:
#Half adder :
module exptwo(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule
#Full adder:
module expthree(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule

```
Logic symbol & Truthtable
RTL realization
![logic](https://user-images.githubusercontent.com/118367518/209817709-03ee8ddb-34dc-4b93-bfa7-773d253a8823.jpg)

### Output:
### RTL
#Half adder:
![image](https://user-images.githubusercontent.com/118367518/209817375-7c0f2c3f-487b-4cd9-b521-14d56633b461.png)
#Full adder:
![image](https://user-images.githubusercontent.com/118367518/209828388-e3a2bba2-160e-42c0-88e9-12bc702d449e.png)

### TIMING DIAGRAM
![image](https://user-images.githubusercontent.com/118367518/209840106-36a27a5a-9b75-4a0e-beb1-4aada47164c7.png)


### TRUTH TABLE 
![image](https://user-images.githubusercontent.com/118367518/209840762-235bf7f0-b9ce-4b8f-8ce0-243eb4f996c4.png)


### Result:
 Thus the half adder and full adder are studied and the truth table for different logic gates are verified.

