## Given an array of strings sorted in lexicographical order, print all of its permutations in strict lexicographical order. If two permutations look the same, only print one of them. See the 'note' below for an example.

Complete the function next_permutation which generates the permutations in the described order.

## For example, s=[ab,bc,cd]. The six permutations in correct order are:

ab bc cd
ab cd bc
bc ab cd
bc cd ab
cd ab bc
cd bc ab
Note: There may be two or more of the same string as elements of .
## For example, s=[ab,bc,cd]. Only one instance of a permutation where all elements match should be printed. In other words, if s[0]==s[1], then print either s[0]  or s[1] but not both.

A three element array having three distinct elements has six permutations as shown above. In this case, there are three matching pairs of permutations where ab and ba are switched. We only print the three visibly unique permutations:

ab ab bc
ab bc ab
bc ab ab
## Input Format

The first line of each test file contains a single integer , the length of the string array .

Each of the next  lines contains a string .

Constraints

 contains only lowercase English letters.
Output Format

Print each permutation as a list of space-separated strings on a single line.

## Sample Input 0

2
ab
cd
## Sample Output 0

ab cd
cd ab
## Sample Input 1

3
a
bc
bc
## Sample Output 1

a bc bc
bc a bc
bc bc a
## AIM:
To write a program to print permutation for the given string.
## ALGORITHM:
1. Start.
2. Define a variables.
3. Write a program to print permutation for the given string.
4. Read the value using scanf.
5. Ask the user to make an input.
6. Print out the answer.
7. End.
## PROGRAM:
```c
#include <stdio.h>
#include <string.h>
void swap(char *x, 
char *y) {
 char temp;
 temp = *x;
 *x = *y;
 *y = temp;
}
void permute(char *str, 
int l, int r) {
 if (l == r) {
 printf("%s\n", str);
 } else {
 for (int i = l; i <= 
r; i++) {
 swap((str + l), 
(str + i)); 
 permute(str, l + 
1, r); 
 swap((str + l), 
(str + i)); 
 }
 }
}
int main() {
 char str[100];
printf("Enter a 
string: ");
 scanf("%s", str);
 int n = strlen(str);
 printf("All 
permutations of the 
string are:\n");
 permute(str, 0, n - 1);
 
 return 0;
}
```
## OUTPUT
Input:

![image](https://github.com/user-attachments/assets/071b5d76-699a-4161-9980-ef45d0eb3e84)

Output:

![image](https://github.com/user-attachments/assets/07b0daf2-5aae-424b-9e1d-1e43a0882ea5)

## RESULT:
Thus, the program is executed and verified successfully.

