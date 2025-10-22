# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    int M, N, i;
    printf("Enter the value of M: ");
    scanf("%d", &M);
    printf("Enter the value of N: ");
    scanf("%d", &N);
    printf("Even numbers from %d to %d are:\n", M, N);
    for (i = M; i <= N; i++) 
    {
        if (i % 2 == 0) 
        {
            printf("%d ", i);
        }
    }
    printf("\n"); 
    return 0;
}

```

## OUTPUT:
<img width="1906" height="1026" alt="Screenshot 2025-10-22 152742" src="https://github.com/user-attachments/assets/61a29086-a7a8-438c-a1dc-6285af0397a7" />











## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include <stdio.h>
int main() 
{
    int n, i, j;
    scanf("%d", &n);
    for (i = 1; i <= n; i++)
    {
        for (j = 1; j <= i; j++) 
        {
            printf("* ");
        }
        printf("\n"); 
    }
    return 0; 
}

```

## OUTPUT:
<img width="1912" height="1031" alt="Screenshot 2025-10-22 153054" src="https://github.com/user-attachments/assets/794b1f10-c2f4-489d-88ab-2058445eca3d" />






## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include <stdio.h>
void addition(int a, int b);
void subtraction(int a, int b);

void addition(int a, int b) 
{
    int sum = a + b;
    printf("Addition of %d and %d = %d\n", a, b, sum);
}
void subtraction(int a, int b)
{
    int diff = a - b;
    printf("Subtraction of %d and %d = %d\n", a, b, diff);
}

int main() 
{
    int num1, num2;
    scanf("%d %d", &num1, &num2);
    addition(num1, num2);
    subtraction(num1, num2);
    return 0;
}

```


## OUTPUT:
<img width="1916" height="1031" alt="Screenshot 2025-10-22 153428" src="https://github.com/user-attachments/assets/0a7052c3-e0c7-46e9-b002-2c52c3b48385" />







## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include <stdio.h>
int main() 
{
    int num,digit, sum = 0;
    scanf("%d", &num);
    for (; num > 0; num = num / 10)
    {
        digit = num % 10; 
        if (digit % 2 != 0) 
        {
            sum += digit;
        }
    }
    printf("Sum of odd digits = %d\n", sum);
    return 0;
}

```


## OUTPUT:
<img width="1919" height="1031" alt="Screenshot 2025-10-22 153813" src="https://github.com/user-attachments/assets/2b5eba3d-b4c2-4171-a294-7c8de8e3a824" />





## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include <stdio.h>
void fact();
int main() 
{
    fact();
    return 0;
}
void fact()
{
    int i, N;
    long long factorial = 1;  
    scanf("%d", &N);
    for (i = 1; i <= N; i++)
    {
        factorial = factorial * i;
    }
    printf("Factorial of %d = %lld\n", N, factorial);
}

```


## OUTPUT:
<img width="1916" height="1030" alt="Screenshot 2025-10-22 154141" src="https://github.com/user-attachments/assets/3af09641-0bba-440b-b956-1c02cabbc059" />


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
