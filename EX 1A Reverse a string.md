# EX 1A Write a Python Program to print factorial of a number recursively.


## DATE:
## AIM:
To write a program to create a factorial of a number recursively.

## Algorithm
1. Input a number num from the user.

2.Check if num is less than 0:

 2.1 If yes, print "Factorial is not defined for negative numbers."

 2.2 If no, proceed to step 4.

3.Define a function factorial(n):

 3.1 If n is 0 or 1, return 1.

 3.2 Else, return n * factorial(n - 1) (i.e., call the function recursively).

4.Call the factorial(num) function.

5.Print the result as "Factorial of number {num} = {result}".
   

## Program:
```
/*
Program to implement Reverse a String
Developed by: Rakesh V
Register Number:  212222110036
*/
```

```
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)

# Taking user input
num = int(input())
if num < 0:
    print("Factorial is not defined for negative numbers.")
else:
    print(f"Factorial of number {num} = {factorial(num)}")
```

## Output:

![image](https://github.com/user-attachments/assets/51885238-0763-4a05-94c7-af8ecde129fd)

# Result:
The program successfully created a factorial of a number using recursion. When the user provides an input number, the output displays the factorial of the number.

