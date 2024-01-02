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
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: S.Sanjay Balaji
RegisterNumber:  23005804
*/
```
HALF ADDER:

module halfadder(a,b,c,s);
input a,b;
output s,c;
xor(s,a,b);
and(c,a,b);
endmodule

FULL ADDER:

module fulladd(a,b,ci,s,Co);
input a,b,ci;
output s,co;
wire d,e,f;
xor(d,a,b);
xor(s,d,ci);
and(e,ci,d);
and(f,a,b);
or(co,e,f);
endmodule
```

### Logic Symbol:
## HALF ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/b204bdcb-024f-47bd-a80b-12e1a1ca33ad)

## FULL ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/ebaf373f-84e6-4776-930c-76be65a3c17b)

### TRUTH TABLE 
## HALF ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/aedd9a7d-1c29-4a5a-9693-ef4c90990056)

## FULL ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/e39a63ed-4e99-4c8d-acdc-4a5d0346631f)

### RTL:
## HALF ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/3c591e53-729b-4671-b75c-cb43b3f51a01)

## FULL ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/7e418470-4d45-4185-86d7-defb882e7398)

### WAVEFORM:
## HALF ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/1d1e5218-eae8-45ac-8acd-a99612bb7439)

## FULL ADDER:
![image](https://github.com/SanjayBalaji0/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/145533553/1b743664-ba97-4408-9b72-4a26507af1e6)

### Result:
Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
