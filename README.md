# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:
LDA 4200H
ΑΝΙ 01H
JZ L1
MVI A, 01H
JMP L2
L1:MVI A, 02H
L2: STA 4201H
HLT

## Output:
ODD
<img width="1693" height="629" alt="Screenshot 2025-08-29 154818" src="https://github.com/user-attachments/assets/f8c45086-b386-4634-9faa-706089dbfb88" />
EVEN
<img width="1700" height="659" alt="Screenshot 2025-08-29 154954" src="https://github.com/user-attachments/assets/0610862d-2d94-4cea-acb6-c8039f4b66f8" />

## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

