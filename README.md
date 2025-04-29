# EX-06 - Looping
## AIM:
Write a C Program to print 1 to n even numbers in reverse order.

## ALGORITHM:
1. Start  
2. Declare an integer variable `n`  
3. Read the value of `n` from the user  
4. Initialize a loop variable `i` with `n`  
5. Repeat while `i >= 1`:  
   - If `i` is even (i.e., `i % 2 == 0`), print `i`  
   - Decrease `i` by 1  
6. End

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    for(int i=n; i>=1; i--)
    if(i%2==0){
        printf("%d ",i);
    }
    
    
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/ab6518e5-0aa6-4ce1-8ac8-e7b58aa328da)

## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:
1. Start  
2. Declare an integer variable `n`  
3. Read the value of `n` (number of rows) from the user  
4. Use a loop to iterate through each row from `1` to `n`  
   - Inside each row, use another loop to print the stars (`*`) for that row  
   - Print the stars based on the current row number  
5. After printing the stars in each row, move to the next line  
6. End


## PROGRAM:
```
#include <stdio.h>
int main() {
   int i, j, rows;
   
   scanf("%d", &rows);
   for (i=rows; i >= 1; i--) {
      for (j = 1; j<=i; j++) {
         printf("$");
      }
      printf("\n");
   }
   return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-29 153512](https://github.com/user-attachments/assets/673a9935-b30f-49ed-a16d-9e708a6ea20b)

## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
# EX-08-Functions

## AIM:
Write a C program to perform multiplication and division of two numbers using functions (with argument and with return type).

## ALGORITHM:
1. Start  
2. Declare two integer variables `a` and `b` for storing the input numbers  
3. Declare two functions: `multiply` and `divide`, each taking two integers as arguments and returning an integer  
   - The `multiply` function will return the product of `a` and `b`  
   - The `divide` function will return the result of dividing `a` by `b`  
4. Read the values of `a` and `b` from the user  
5. Call the `multiply` function with `a` and `b` as arguments, and store the result  
6. Call the `divide` function with `a` and `b` as arguments, and store the result  
7. Print the multiplication and division results  
8. End


## PROGRAM:
```
#include <stdio.h>
int multiply(int a, int b) {
    return a * b;
}
float divide(int a, int b) {
    return (float)a / b;
}

int main() {
    int num1, num2;
    scanf("%d %d", &num1, &num2);
    printf("Multiplication: %d\n", multiply(num1, num2));
    printf("Division: %f\n", divide(num1, num2));
    
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/210567d8-5c36-40de-b44a-1730c8a9059d)

## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop in a given range

## ALGORITHM:

1. Start  
2. Declare integer variables `start`, `end`, and `sum`  
3. Read the values of `start` and `end` (the range) from the user  
4. Initialize `sum` to 0  
5. Use a `for` loop to iterate from `start` to `end`  
   - For each number in the range, extract each digit  
   - If the digit is odd (i.e., `digit % 2 != 0`), add it to `sum`  
6. After the loop, print the value of `sum`  
7. End

## PROGRAM:
```
#include <stdio.h>

int main() {
    int start, end, sum = 0;
    scanf("%d", &start);
    scanf("%d", &end);
    for (int i = start; i <= end; i++) {
        if (i % 2 != 0) { 
            printf("%d  ", i);
            sum += i; 
        }
    }

    printf("\n%d\n", sum); 

    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/22d3ee5f-6773-4b65-960e-f0d3047251b8)

## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.

# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1. Start  
2. Declare an integer variable `n` to store the input number  
3. Read the value of `n` from the user  
4. Define a function `factorial` that takes an integer argument and returns the factorial  
   - Inside the function, use a loop to calculate the factorial  
   - Return the factorial value  
5. Call the `factorial` function with `n` as the argument and store the result  
6. Print the result (factorial)  
7. End

## PROGRAM:
```
#include <stdio.h>
unsigned long long factorial(int n) {
    if (n < 0) {
        return 0;
    }
    
    unsigned long long fact = 1;
    for (int i = 1; i <= n; i++) {
        fact *= i;
    }
    return fact;
}

int main() {
    int num;
    scanf("%d", &num);
    printf("Factorial value is: %llu\n", factorial(num));
    
    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/c01d25e1-a66e-4ad7-9d3d-f788a68fac37)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
