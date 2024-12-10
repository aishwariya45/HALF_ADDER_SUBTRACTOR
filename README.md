# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER
![image](https://github.com/user-attachments/assets/5a5e10b9-c153-40e1-b671-ce7ca2bae50a)
![image](https://github.com/user-attachments/assets/69e0c514-efaa-4b75-a08e-1e36e8c2fc8f)



**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)
 

Figure -02 HALF Subtractor



**Truthtable**
![image](https://github.com/user-attachments/assets/ec214897-6bfe-4690-9dff-b2d9e2210799)
![image](https://github.com/user-attachments/assets/0a00b0ee-acc4-4e82-9a13-d9a142099a7e)



**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:S>AISHWARIYA RegisterNumber:24900840
```
module exp31(a,b,cy,sm,df,bo);
input a,b;
output sm,cy,df,bo;
xor(sm,a,b);
and(cy,a,b);
xor(df,a,b);
and(bo,~a,b);
endmodule
```

**RTL Schematic**
![exp31](https://github.com/user-attachments/assets/9d42b514-6154-416b-91b2-264269175971)


**Output/TIMING Waveform**
![Screenshot 2024-12-10 111952](https://github.com/user-attachments/assets/c0c8df6c-5358-4708-b35a-094afc0abe04)


**Result:**
true table of half adder and full adder are verified successfully
