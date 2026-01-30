# Python Functions, Loops & Logic Practice 🐍

This repository contains **Python practice examples and notebook exercises** focused on building a strong foundation in **functions**, **loops**, **indentation**, and **logic-based problem solving**.

It also includes **Reeborg’s World challenges** (Hurdles & Maze) to practice real problem-solving using conditions and loops.

These exercises are ideal for **Python beginners** learning how to write clean, reusable, and logical code.

---

## Topics Covered

### Python Functions

* What a function is
* Why functions are useful
* Defining functions using `def`
* Calling functions
* Code reusability

**Example**

```python
def my_function():
    print("Hello")
    print("Bye")

my_function()
```

---

### Indentation in Python

* Understanding Python’s indentation rules
* How indentation defines code blocks
* Common indentation mistakes

**Example**

```python
def my_function():
    print("Michel")
    print("&")
    print("Sam")

print("Bye!")
my_function()
```

---

### While Loops

* What a `while` loop is
* Looping until a condition becomes false
* Manual counting using a loop

**Example**

```python
i = 0
while i < 10:
    print(i)
    i += 1
```

---

### For Loops

* Iterating using `range()`
* Understanding start, stop values
* Repeating actions efficiently

**Example**

```python
for i in range(1, 11):
    print(i)
```

---

## Reeborg’s World Challenges 🤖

These exercises use **Reeborg’s World** to practice movement logic, conditions, and loops.

---

### Alone Challenge

* Creating helper functions
* Breaking down repeated movements
* Improving readability

---

### Hurdle 1

* Writing movement functions
* Manually calling functions
* Using loops to reduce repetition

**Concepts Used**

* Functions
* While loops
* Counters

---

### Hurdle 2

* Using `while not at_goal()`
* Letting the robot run until the goal is reached
* Cleaner logic without hard-coding steps

---

### Hurdle 3

* Using `if / else` conditions
* Detecting walls with `wall_in_front()`
* Making decisions dynamically

---

### Hurdle 4

* Handling variable hurdle heights
* Nested loops
* Advanced movement logic

**Concepts Used**

* Nested `while` loops
* Conditional checks
* Reusable functions

---

### Maze Solver

* Solving a maze using the **right-hand rule**
* Making decisions based on surroundings

**Logic Used**

* `right_is_clear()`
* `front_is_clear()`
* `turn_left()` and custom `turn_right()`

---

## How to Run the Notebook

### Using Jupyter Notebook

1. Install Jupyter (if not installed):

   ```bash
   pip install notebook
   ```
2. Start Jupyter:

   ```bash
   jupyter notebook
   ```
3. Open the `.ipynb` file
4. Run cells step by step

---

## Learning Objectives

By completing this notebook, you will:

* Understand how Python functions work
* Write clean and reusable code
* Master `for` and `while` loops
* Learn proper indentation and code structure
* Apply logic using conditions
* Solve problems step by step
* Improve algorithmic thinking

---

## Ideal For

* Python beginners
* Students learning programming basics
* Anyone practicing loops and functions
* Learners using Reeborg’s World challenges

---

