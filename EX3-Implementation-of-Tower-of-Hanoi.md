# EX3 Implementation of Tower of Hanoi
## DATE:2.5.2025
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Start the program.
2.Define the priority() function to return the priority of operators.
.Initialize the string containing operators and operands.
4.Loop through each character in the string.
5.For each operator, call the priority() function to determine its priority.
6.Print the operator and its corresponding priority level.
7.End
     

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: DEVA DHARSHINI.I
RegisterNumber: 212223240026
*/
```
```
#include <stdio.h>

void TOH(int n, char source, char dest, char aux) {
    if (n == 1) {
        printf("%c to %c\n", source, dest);
        return;
    }
    TOH(n - 1, source, aux, dest);
    printf("%c to %c\n", source, dest);
    TOH(n - 1, aux, dest, source);
}
```

## Output:
![Screenshot 2025-05-05 111758](https://github.com/user-attachments/assets/43a5510b-ed98-459e-bd35-a67bb8c0633f)



## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
