# Find the square root of a number

## AIM:
To write a program to find the square root of a number.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Define a function.
2. Assign number_iters = 100 in the function to perform 100 iteratios.
3. Set i = 0.
4. Calculate  number = 0.5 * (number + a / number) for 100 iterations.
5. Return number

## Program:
```
/*
Program to find the square root for the given number(newton's method) using function.
Developed by: Sri Saran J
RegisterNumber:  212225240159
*/
```def sqrt_newton(b, tolerance=1e-10):
    if b == 0:
        return 0.0
    
    x = b / 2.0  # initial guess
    
    while True:
        next_x = 0.5 * (x + b / x)
        if abs(next_x - x) < tolerance:
            return next_x
        x = next_x

# Driver code
num = float(input())
print("Square root of the number:", sqrt_newton(num))


## Output:

<img width="1170" height="279" alt="image" src="https://github.com/user-attachments/assets/f68f205c-0e4d-40c8-ab79-c9be8e46d93a" />


## Result:
Thus the program to find the square root for the given number(newton's method) using function is written and verified using python programming.
