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


**PROGRAM**

Program for logic gates and verify its truth table in quartus using Verilog programming
```
Developed by:Tharun.B
RegisterNumber:212224240171
```
```py
module LOGIC_GATES(a,b,andgate,orgate,notgate,nandgate,norgate,xorgate,xnorgate);
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

**Logic symbol & Truthtable**

![image](https://github.com/gauthamkrishna7/study-of-basic-gates/assets/141175025/2f6d090e-b158-4a7f-a95c-8607e599e91a)

![image](https://github.com/gauthamkrishna7/study-of-basic-gates/assets/141175025/40baeb41-c5d7-4de3-be03-c21544a9419a)


**RTL realization:**

![image](https://github.com/gauthamkrishna7/study-of-basic-gates/assets/141175025/ec8c42e3-917f-4019-a1f5-a31d00f47b32)

 
**Output:** 

![image](https://github.com/gauthamkrishna7/study-of-basic-gates/assets/141175025/0cceb6d6-38dd-4eca-a70e-df1b7f5cfdca)


**Result:**

Thus the different digital IC’s are studied and the truth table for different logic gates are verified.


