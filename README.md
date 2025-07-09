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

```
##🛠 How to Run
#Clone this repository
```
git clone https://github.com/hemant2871/c-projects.git
cd c-projects
```

#Compile the code
```
gcc calculator.c -o calculator
```
#Run the program

```
./calculator
```
##📂 Upcoming Projects
1.Number Guessing Game

2.Armstrong Number Checker

3.Prime Number Generator

4.Pattern Printing

5.Tic-Tac-Toe in C (console)

More interesting logic-based mini projects...

##📧 Contact
Created with 💻 by Hemant Sharma
📫 Reach out via [LinkedIn](www.linkedin.com/in/hemant-sharma-3135b4290) or [GitHub](https://github.com/hemant2871) 
