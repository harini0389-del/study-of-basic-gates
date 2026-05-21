### study-of-basic-gates

**AIM:** 

To study and verify the truth table of logic gates in Quartus II using Verilog programming.

**Equipments Required:**

Software – Quartus prime 

**Theory**

Introduction Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as

AND gate OR gate NOT gate NAND gate NOR gate Ex-OR gate Ex-NOR gate

**AND gate**

The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B

**OR gate** 

The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B

**NOT gate**

The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'

**NAND gate**

This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’

**NOR gate**

This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’

**Ex-OR gate**

The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B

**Ex-NOR gate**

The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B

**Procedure** 

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**PROGRAM**module logicgates1(a, b, c);
    input a;
    input b;
    output  [6:0] c;
```
module exp1(a,b,andgate,orgate,notgate,nandgate,norgate,xorgate,xnorgate);
input a,b;
output andgate,orgate,notgate,nandgate,norgate,xorgate,xnorgate;
and(andgate,a,b);
or(orgate,a,b);
not(notgate,a);
nand(nandgate,a,b);
nor(norgate,a,b);
xor(xorgate,a,b);
xnor(xnorgate,a,b);
endmodule
```
Program for logic gates and verify its truth table in quartus using Verilog programming

 Developed by:Harini M RegisterNumber:212225240047
 
**Logic symbol & Truthtable**
<img width="815" height="597" alt="image" src="https://github.com/user-attachments/assets/4515c528-e101-4dc1-bfc6-38ca5031820f" />
<img width="852" height="440" alt="image" src="https://github.com/user-attachments/assets/568e0377-1da8-4879-88d7-6cbbb4452b5e" />

**RTL realization Output:** 
<img width="737" height="562" alt="image" src="https://github.com/user-attachments/assets/1005e861-36b0-43f2-b0e4-65eccbaca3fa" />

**RTL**
<img width="1242" height="307" alt="image" src="https://github.com/user-attachments/assets/8cdc6cc0-5a34-4f8b-a850-94d66b8dde3b" />

**Result:**
Thus the outputs of Basic Logic Gates are verified by simulating and synthesizing the VERILOG code.

