#  Python Basics & Mini Projects

This repository contains my Python learning journey, starting from basic functions to small logical programs like a **Prime Number Checker** and a **Caesar Cipher**.
It is mainly focused on understanding **functions, arguments, loops, and conditionals**.



##  Topics Covered

*  Python Functions
*  Positional & Keyword Arguments
*  User Input Handling
*  Basic Math Calculations
*  Loops & Conditional Statements
*  Error Handling (basic)
*  Mini Projects



##  Programs Included

### 1️. Hello World & Functions

Basic examples of:

* Defining functions
* Calling functions
* Using `__main__`

```python
def greet():
    print("Hello, World!")
```



### 2️. Function with Parameters

Using arguments and parameters in functions.

```python
def greet(name, age):
    print(f"Hello, {name}!")
    print(f"You are {age} years old.")
```



### 3️. Paint Can Calculator 

Calculates the number of paint cans required based on height, width, and coverage.

```python
def no_of_cans(height, width, coverage):
    cans = (height * width) / coverage
    print(round(cans))
```



###  Prime Number Checker 

Checks whether a given number is prime or not.

```python
def prime_checker(number):
    is_prime = True
    for i in range(2, number):
        if number % i == 0:
            is_prime = False
```


###  Caesar Cipher 

A simple encryption and decryption program using the Caesar Cipher technique.

**Features:**

* Encode and Decode messages
* Custom shift value
* Handles lowercase letters

```python
def caser(start_text, shift_amount, direction):
    ...
```

**Note:**
The current version throws an error when spaces or special characters are used (`' ' is not in list`).
This can be fixed by adding a condition to skip non-alphabet characters.



##  How to Run

1. Clone the repository

```bash
git clone https://github.com/your-username/repo-name.git
```

2. Run the Python file or open the notebook

```bash
python filename.py
```

---

##  Requirements

* Python 3.11+
* No external libraries required (except `art` module for logo display in Caesar Cipher)



##  Learning Goal

This repository is part of my journey to:

* Build strong Python fundamentals
* Practice logic building
* Prepare for advanced Python concepts

