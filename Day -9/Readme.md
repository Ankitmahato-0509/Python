# Day 9 – Python Dictionaries & Mini Project

This notebook is part of my **Python learning journey** and focuses on **Dictionaries, Nested Data, Loops, and Data Manipulation**.

The notebook also includes a practical **Blind Auction** mini project using dictionaries, loops, functions, and user input.



##  Topics Covered

- Python Dictionaries
- Creating and accessing dictionaries
- Adding new items to a dictionary
- Editing dictionary values
- Creating empty dictionaries
- Looping through dictionaries
- Nested dictionaries
- Lists inside dictionaries
- Dictionaries inside lists
- Working with user input
- Functions with dictionaries
- Conditional statements
- Finding the highest value
- Mini Project – Blind Auction



## 1. Python Dictionaries

A dictionary stores data in **key-value pairs**.

### Example

```python
programming_dictionary = {
    "Bug": "An error in a program that prevents the program from running as expected.",
    "Function": "A piece of code that you can easily call over and over again."
}

print(programming_dictionary["Function"])
````



## 2. Adding Items to a Dictionary

New key-value pairs can be added to an existing dictionary.

```python
programming_dictionary["Loop"] = "The action of doing something over and over again."

print(programming_dictionary)
```



## 3. Creating an Empty Dictionary

```python
empty_dictionary = {}
```

An empty dictionary can later be populated with data.



## 4. Editing Dictionary Values

Dictionary values can be updated using their keys.

```python
programming_dictionary["Bug"] = "A moth in your computer."
```



## 5. Looping Through a Dictionary

A `for` loop can be used to access dictionary keys and values.

```python
for key in programming_dictionary:
    print(key)
    print(programming_dictionary[key])
```



## 6. Student Grades

A dictionary containing student scores is converted into a new dictionary containing grade categories.

### Grade Categories

* `91+` → Outstanding
* `81–90` → Exceeds Expectations
* `71–80` → Acceptable
* Below `71` → Fail

```python
for student in student_scores:
    score = student_scores[student]

    if score >= 91:
        student_grades[student] = "Outstanding"
    elif score >= 81:
        student_grades[student] = "Exceeds Expectations"
    elif score >= 71:
        student_grades[student] = "Acceptable"
    else:
        student_grades[student] = "Fail"
```

The notebook produces the final `student_grades` dictionary. 



## 7. Nested Data

The notebook demonstrates different ways of storing related data.

### Dictionary with a List

```python
travel_log = {
    "France": ["Paris", "Lille", "Dijon"],
    "Germany": ["Berlin", "Hamburg", "Stuttgart"]
}
```

### Nested Dictionary

```python
travel_log = {
    "France": {
        "cities_visited": ["Paris", "Lille", "Dijon"],
        "total_visits": 12
    },
    "Germany": {
        "cities_visited": ["Berlin", "Hamburg", "Stuttgart"],
        "total_visits": 5
    }
}
```

These examples demonstrate how dictionaries can contain lists and other dictionaries. 



## 8. Dictionary Inside a List

The notebook also demonstrates storing multiple dictionaries inside a list.

```python
travel_log = [
    {
        "country": "France",
        "cities_visited": ["Paris", "Lille", "Dijon"],
        "total_visits": 12
    },
    {
        "country": "Germany",
        "cities_visited": ["Berlin", "Hamburg", "Stuttgart"],
        "total_visited": 5
    }
]
```



## 9. Adding a New Country

A function is used to add a new country and its travel information to the `travel_log`.

```python
def add_new_country(country_visited, time_visited, cities_visited):
    new_country = {}
    new_country["Country"] = country_visited
    new_country["Visits"] = time_visited
    new_country["cities"] = cities_visited

    travel_log.append(new_country)
```

Example:

```python
add_new_country(
    "Russia",
    2,
    ["Moscow", "Saint Petersberg"]
)
```

The new country is then added to the travel log. 



#  Mini Project – Blind Auction

The notebook includes a **Blind Auction** project.

The program allows multiple bidders to enter their names and bid amounts. The bids are stored inside a dictionary.

```python
bids = {}
```

A function is used to find the bidder with the highest bid.

```python
def find_highest_bidder(bidding_record):
    highest_bid = 0
    winner = ""

    for bidder in bidding_record:
        bid_amount = bidding_record[bidder]

        if bid_amount > highest_bid:
            highest_bid = bid_amount
            winner = bidder

    print(f"The winner is {winner} with a bid of ${highest_bid}")
```

The program continues accepting bids until the user enters `"no"` when asked whether there are other bidders. 

### Example Output

```text
The winner is kelvin with a bid of $500.0
```



## Key Learning

Through this notebook, I practiced:

* Creating dictionaries
* Accessing dictionary values
* Adding and updating data
* Looping through dictionaries
* Using conditional statements with dictionaries
* Working with nested data
* Combining lists and dictionaries
* Creating functions to manipulate dictionary data
* Taking user input
* Finding the highest value in a dictionary
* Building a practical mini project


## Skills Practiced

* Python
* Dictionaries
* Lists
* Loops
* Functions
* Conditional Statements
* User Input
* Nested Data Structures
* Logic Building
* Problem Solving

##  Requirements

* Python 3.11+
* Jupyter Notebook / JupyterLab / VS Code
* `art` module for the Blind Auction logo


## Learning Goal

This notebook is part of my Python learning journey to:

* Strengthen Python fundamentals
* Understand data structures
* Improve logical thinking
* Practice problem solving
* Build small Python projects
* Prepare for more advanced Python concepts

```
