# # Task

# # Given a positive integer denoting , do the following:

# If  41<=n <=49 print the lowercase English word corresponding to the number (e.g., forty one for 41 , forty two for 42 etc.).
If n>49 print Greater than 49.
## Input Format

The first line contains a single integer, .

## Constraints

## Output Format

If  41<=n <=49 print the lowercase English word corresponding to the number (e.g., forty one for 4 , forty two for 42 etc.).
If n>49 print Greater than 49.
## Sample Input

41
## Sample Output

forty one
## Sample Output

forty one

## AIM:
To write a program to print the English word corresponding to the given number.

## ALGORITHM:
1. Start.
2. Define a variables.
3. Write a program to print the English word corresponding to the given number.
4. Read the value using scanf.
5. Ask the user to make an input.
6. Print out the answer.
7. End.
   
## PROGRAM:
```c
#include <stdio.h>
int main() {
 int num;
 scanf("%d", &num);
 switch (num) {
 case 41: 
printf("forty one\n"); break;
 case 42: 
printf("forty two\n"); break;
 case 43: 
printf("forty three\n"); 
break;
 case 44: 
printf("forty four\n"); break;
 case 45: 
printf("forty five\n"); break;
 case 46: 
printf("forty six\n"); break;
 case 47: 
printf("forty seven\n"); 
break;
 case 48:
printf("forty eight\n"); 
break;
 case 49: 
printf("forty nine\n"); break;
 default: 
printf(" Greater than 49\n"); break;
 }
 return 0;
}
```
## OUTPUT
![Screenshot 2025-05-13 183348](https://github.com/user-attachments/assets/c00fe928-a351-4f09-95b0-52af7c7a66f6)
## RESULT:
Thus, the program is executed and verified successfully

