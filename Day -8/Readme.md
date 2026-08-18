
# Python Basics & Mini Projects

This repository contains my Python learning journey, starting with basic functions and progressing to small logical programs and mini projects.

The main focus is on understanding **functions, parameters, arguments, user input, loops, conditional statements, and basic problem-solving**.

##  Topics Covered

- Python Functions
- Positional Arguments
- Keyword Arguments
- User Input
- Basic Math Calculations
- Loops
- Conditional Statements
- Boolean Logic
- String Manipulation
- Mini Projects
- Encryption & Decryption


##  Programs Included

### 1. Hello World & Functions

Basic practice with defining and calling Python functions.

```python
def greet():
    print("Hello, World!")
````

**Concepts Learned:**

* Defining functions
* Calling functions
* Using `__main__`
* Printing output



### 2. Functions with Parameters

Practiced creating functions that accept parameters and arguments.

```python
def greet(name, age):
    print(f"Hello, {name}!")
    print(f"You are {age} years old.")
```

**Concepts Learned:**

* Parameters
* Arguments
* Multiple parameters
* Passing values to functions



### 3. Positional & Keyword Arguments

Practiced passing values using both positional and keyword arguments.

```python
greet("Ankit", 25)

greet(name="Ankit", age=25)
```

**Concepts Learned:**

* Positional arguments
* Keyword arguments
* Named parameters



##  4. Paint Can Calculator

A small program that calculates the number of paint cans required based on height, width, and coverage.

### Formula

```text
Number of Cans = (Height × Width) / Coverage
```

### Example

```python
def no_of_cans(height, width, coverage):
    cans = (height * width) / coverage
    print(round(cans))
```

**Concepts Learned:**

* Functions
* Parameters
* Mathematical calculations
* `round()`
* Formatted output



##  5. Prime Number Checker

A program that checks whether a given number is a prime number.

```python
def prime_checker(number):
    is_prime = True

    for i in range(2, number):
        if number % i == 0:
            is_prime = False

    if is_prime:
        print("It's a prime number.")
    else:
        print("It's not a prime number.")
```

**Concepts Learned:**

* `for` loops
* `range()`
* Modulo operator `%`
* Conditional statements
* Boolean variables
* Logical problem-solving



##  6. Caesar Cipher

A simple encryption and decryption program based on the **Caesar Cipher** technique.

### Features

* Encode messages
* Decode messages
* Custom shift value
* Handle lowercase letters
* Preserve spaces and other characters
* User input
* Encryption and decryption logic

**Concepts Learned:**

* String manipulation
* Lists
* Loops
* Conditional statements
* Functions
* User input
* Encryption
* Decryption

##  Requirements

* Python 3.11+
* Jupyter Notebook
* `art` module for the Caesar Cipher logo


## Learning Goals

Through these exercises, I am working toward:

* Building strong Python fundamentals
* Understanding functions and arguments
* Improving logical thinking
* Practicing problem-solving
* Understanding loops and conditions
* Learning basic encryption concepts
* Building small Python projects
* Preparing for advanced Python and Data Analytics concepts




## Project Status

**Status:** Completed

This repository represents my practice with Python fundamentals and beginner-level mini projects.
