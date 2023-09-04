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
```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: NAGUL K
RegisterNumber:  212222230089
```
## Half Adder
```
module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule
```

## Full Adder
```
module exp3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry=(a&b)|((a^b)&c);
endmodule
```
# TRUTH TABLE
## HALF ADDER
![image](https://github.com/Nagul71/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118661118/4cfcba24-d1a1-42be-8f2d-c1f64f7d9b3f)
## FULL ADDER
![image](https://github.com/Nagul71/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118661118/2b71bdd5-7bdf-430a-87f7-486f27029265)


# RTL
## Half Adder
![Screenshot 2023-09-02 092308](https://github.com/Nagul71/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118661118/4d0a6317-9091-4188-bb7c-ed0f65ccf829)


## Full Adder
![Screenshot 2023-09-02 093119](https://github.com/Nagul71/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118661118/10e0c376-d39b-4071-915c-a567ba3f1f8c)



# TIMING DIAGRAM
## Half Adder
![image](https://github.com/Nagul71/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118661118/ca504da7-ffee-40ee-8fd4-792c090bb418)



## Full Adder

![Screenshot 2023-09-02 093821](https://github.com/Nagul71/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/118661118/2b40d1a2-09bf-4d3d-be7e-e1455146fa98)



# Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.
