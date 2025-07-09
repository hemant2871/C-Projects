# C Projects 🚀

Welcome to my C Projects repository! This space is dedicated to storing various logic-based mini projects and programs created using the C programming language. Whether you're a beginner looking for examples or someone revisiting C, this repo has something for you.

## 📌 Project 1: Simple Calculator

A command-line calculator built using C that supports basic arithmetic operations: addition, subtraction, multiplication, and division.

### 🔧 Features
- Takes user input for operator and operands.
- Performs calculation based on selected operation.
- Handles division by zero errors gracefully.
- Simple and clean user interface via terminal.

### 📄 Code Example

```c
#include <stdio.h>

int main() {
    char operator;
    double firstNumber, secondNumber;

    printf("Enter an operator (+, -, *, /): ");
    scanf("%c", &operator);

    printf("Enter two operands: ");
    scanf("%lf %lf", &firstNumber, &secondNumber);

    switch (operator) {
        case '+':
            printf("%.2lf + %.2lf = %.2lf\n", firstNumber, secondNumber, firstNumber + secondNumber);
            break;
        case '-':
            printf("%.2lf - %.2lf = %.2lf\n", firstNumber, secondNumber, firstNumber - secondNumber);
            break;
        case '*':
            printf("%.2lf * %.2lf = %.2lf\n", firstNumber, secondNumber, firstNumber * secondNumber);
            break;
        case '/':
            if (secondNumber != 0)
                printf("%.2lf / %.2lf = %.2lf\n", firstNumber, secondNumber, firstNumber / secondNumber);
            else
                printf("Error! Division by zero.\n");
            break;
        default:
            printf("Error! Operator is not correct\n");
    }

    return 0;
}
