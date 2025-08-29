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
<img width="1693" height="629" alt="Screenshot 2025-08-29 154818" src="https://github.com/user-attachments/assets/10a805d0-1f34-4382-85e4-d0efd81f3bf2" />
EVEN
<img width="1700" height="659" alt="Screenshot 2025-08-29 154954" src="https://github.com/user-attachments/assets/ebee83a5-20f6-400e-9d08-314c0e0b65c1" />



## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

