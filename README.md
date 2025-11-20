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

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
HALF ADDER :
<img width="409" height="229" alt="Screenshot 2025-11-20 205553" src="https://github.com/user-attachments/assets/225abe72-2588-41a1-a58a-b1dd3b5913fd" />

HALF SUBTRATER :

<img width="423" height="232" alt="Screenshot 2025-11-20 205613" src="https://github.com/user-attachments/assets/a064df86-beec-46f8-a1ed-29b446a7c6b6" />


**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:NIVETHA.S.K RegisterNumber:25016594

HALF ADDER :
module half_adder(sum, carry, a, b);
  output sum;
  output carry;
  input a;
  input b;
  assign sum = a ^ b;
  assign carry = a & b;
endmodule

HALF SUBTRACTER :

module half_subtractor(diff, borrow, a, b);
  output diff;
  output borrow;
  input a;
  input b;
  assign diff = a ^ b;
  assign borrow = ~a & b;
endmodule

**RTL Schematic**

HALF ADDER :
<img width="833" height="367" alt="Screenshot 2025-11-20 205735" src="https://github.com/user-attachments/assets/d2359fcb-943e-4b97-b52d-6039b8963159" />

HALF SUBTRACTER :
<img width="787" height="348" alt="Screenshot 2025-11-20 205745" src="https://github.com/user-attachments/assets/4522355f-3ac6-4982-b674-a6a43444a647" />


**Output/TIMING Waveform**

HALF ADDER :
<img width="953" height="478" alt="Screenshot 2025-11-20 205835" src="https://github.com/user-attachments/assets/96dab05f-8cb1-47aa-ad07-e506e06f9686" />

HALF SUBTRACTER :
<img width="828" height="321" alt="Screenshot 2025-11-20 205927" src="https://github.com/user-attachments/assets/0b3bcc1f-b38f-46e9-aa5a-204979544117" />

**Result:**

Half adder and half subtractor circuit its truth table in Quartus using Verilog programming verified successfully .
