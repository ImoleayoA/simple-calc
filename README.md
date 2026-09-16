# Simple Calculator

A beginner-friendly command-line calculator built with Python.

The program accepts two numbers and an arithmetic operator, performs the selected calculation, handles invalid input, prevents division by zero, and allows the user to continue or exit.

## Features

* Addition (`+`)
* Subtraction (`-`)
* Multiplication (`*`)
* Division (`/`)
* Division-by-zero protection
* Invalid operator validation
* Number input validation
* Continue or exit option
* Accepts `y`, `yes`, `n`, or `no`
* Handles `Ctrl+C` and `EOF` gracefully

## Requirements

* Python 3.x
* No external libraries are required.

## How to Run

1. Make sure Python is installed:

```bash
python3 --version
```

2. Run the program:

```bash
python3 calculator.py
```

Replace `calculator.py` with the actual name of your Python file if different.

## How It Works

The calculator follows these steps:

1. Asks the user for the first number.
2. Asks for an operator:

   * `+`
   * `-`
   * `*`
   * `/`
3. Checks whether the operator is valid.
4. If the operator is valid, asks for the second number.
5. Performs the selected calculation.
6. Prevents division by zero.
7. Asks whether the user wants to continue.
8. Continues when the user enters `y` or `yes`.
9. Exits when the user enters `n` or `no`.

## Example

```text
Enter first number: 15
Enter operator from the following (+, -, *, /): *
Enter second number: 4
60.0
Do you want to continue? (y/n) or (yes/no): y

Enter first number: 20
Enter operator from the following (+, -, *, /): /
Enter second number: 0
Cannot divide by zero
Do you want to continue? (y/n) or (yes/no): no
Exiting the calculator...
```

## Input Validation

### Invalid Number

If the user enters something that cannot be converted to a number:

```text
Enter first number: hello
Please enter a valid number
```

### Invalid Operator

If the user enters an unsupported operator:

```text
Enter operator from the following (+, -, *, /): %
Invalid operator. Please enter an operator from the following (+, -, *, /)
```

### Division by Zero

The program checks the second number before performing division:

```text
Enter first number: 20
Enter operator from the following (+, -, *, /): /
Enter second number: 0
Cannot divide by zero
```

### Continue or Exit

The program accepts:

```text
y
yes
n
no
```

Any other response is rejected:

```text
Please enter y/n or yes/no
```

## Concepts Practiced

This project practices several fundamental Python concepts:

* `input()`
* Type conversion with `float()`
* `if / elif / else`
* `while` loops
* `break`
* Membership testing with `in`
* Tuples
* String methods:

  * `.strip()`
  * `.lower()`
* `try / except`
* `ValueError`
* `KeyboardInterrupt`
* `EOFError`
* Basic arithmetic operators

## Project Goal

This project was created as a beginner Python exercise to practice control flow, input validation, loops, exception handling, and basic arithmetic operations.

