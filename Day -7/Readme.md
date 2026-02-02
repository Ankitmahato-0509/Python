# Python Functions, Loops & Logic Practice

This repository contains **Python practice examples and notebook exercises** focused on building a strong foundation in **functions, loops, indentation, and logic-based problem solving**. 

It includes **complete Hangman game development** (5 progressive steps) and **Reeborg's World challenges** (Hurdles & Maze) to practice real problem-solving using conditions and loops.

These exercises are ideal for **Python beginners** learning how to write clean, reusable, and logical code.

##  Table of Contents
- [Hangman Game](#hangman-game)
- [Topics Covered](#topics-covered)
- [Reeborg's World Challenges](#reeborgs-world-challenges)
- [How to Run](#how-to-run)
- [Learning Objectives](#learning-objectives)


##  Hangman Game
**Complete implementation** through 5 progressive steps:

| Step | Features Added |
|------|----------------|
| **Step 1** | Random word selection, single letter guessing |
| **Step 2** | Display blanks, reveal correct letters |
| **Step 3** | While loop for multiple guesses |
| **Step 4** | Lives system + ASCII hangman art |
| **Step 5** | Duplicate guess handling, external word lists |

**Live Demo Output:**
```
_ a _ _ r _ _ _ _ _
  +---+
  |   |
      |
      |
      |
      |
=========
You've already guessed e
w a t e r _ e _ _ _
```

##  Topics Covered

### Python Functions
- What functions are & why they're useful
- Defining functions using `def`
- Calling functions & code reusability

```python
def my_function():
    print("Hello")
    print("Bye")

my_function()
```

### Indentation in Python
- Python's indentation rules
- How indentation defines code blocks
- Common indentation mistakes

### While Loops
- Looping until condition becomes false
- Manual counting using loops

```python
i = 0
while i < 10:
    print(i)
    i += 1
```

### For Loops
- Iterating using `range()`
- Understanding start, stop values

```python
for i in range(1, 11):
    print(i)
```

##  Reeborg's World Challenges

### Alone Challenge
- Creating helper functions
- Breaking down repeated movements

### Hurdle Challenges (1-4)
```
Hurdle 1: Basic movement + loops
Hurdle 2: while not at_goal()
Hurdle 3: if/else + wall_in_front()
Hurdle 4: Variable heights + nested loops
```

### Maze Solver
- Right-hand rule algorithm
- `right_is_clear()`, `front_is_clear()`
- Custom `turn_right()` function

##  How to Run

### Jupyter Notebook
```bash
pip install notebook
jupyter notebook
# Open .ipynb & run cells step-by-step
```

### Google Colab
- Open in [Google Colab](https://colab.research.google.com)
- Run cells sequentially

##  Learning Objectives
By completing this notebook, you will:
-  Master Python functions
-  Write clean, reusable code
-  Master `for`/`while` loops
-  Perfect indentation & structure
-  Apply `if/else` conditions
-  Solve problems step-by-step
-  Build algorithmic thinking


***

⭐ **Star if helpful!**  
📚 **For Python learners**
