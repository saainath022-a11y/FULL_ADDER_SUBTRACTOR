# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**
<img width="242" height="173" alt="527463664-1d3f28da-0ff9-48fc-8dde-237c8238e469" src="https://github.com/user-attachments/assets/1d6d1272-a869-4a98-95c0-3e91487153c6" />

**Procedure**

Write the detailed procedure here

**Program:**
```
Developed by: SAAIANTH B 
RegisterNumber: 25016015

module ex4 (a,b,c,x,y,z,sum,dif,car,bor);
input a,b,c,x,y,z;
output sum,dif,car,bor;
assign sum = a^b^c;
assign car = a&b | a&c | b&c;
assign dif = x^y^z;
assign bor = ~x&z | ~x&y | y&z;
endmodule

```
/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming. Developed by: RegisterNumber:
*/

**RTL Schematic**
<img width="1555" height="861" alt="523423590-f7a8696e-4908-4dec-89f4-8e5faddf7a01" src="https://github.com/user-attachments/assets/01ed220b-f462-4a46-a3d5-6e0a71368503" />

**Output Timing Waveform**
<img width="1645" height="625" alt="523423598-02c78151-1592-43f1-a355-332d96155492" src="https://github.com/user-attachments/assets/629beda8-a906-457c-b515-44f642562f70" />

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



