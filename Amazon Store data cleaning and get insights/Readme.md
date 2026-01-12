
# Amazon Store Data Analysis

A practical Python project demonstrating data cleaning, analysis, and basic recommendation logic using customer review data stored in JSON format.

-

## Overview

This repository contains a Jupyter notebook and a sample JSON dataset used to analyze customer feedback from an Amazon-like online store.  
The project focuses on:
- Cleaning inconsistent real-world data
- Handling missing and duplicate values
- Deriving meaningful insights from customer ratings
- Generating simple brand recommendations

-

## Contents

### Main Files

1. **Amazon-Store-data.ipynb**
   - Jupyter notebook with step-by-step data analysis
   - Loads JSON data using Python’s `json` module
   - Cleans inconsistent ratings (text → numeric)
   - Handles missing values (e.g., age)
   - Removes duplicate customer entries
   - Computes statistics and generates recommendations

2. **store_data.json**
   - Sample JSON dataset with 6 customer reviews
   - Fields included:
     - `name` – Customer name
     - `rating` – Numeric or text-based rating
     - `feedback` – Customer feedback text
     - `age` – Customer age (some values missing)

-

## Key Concepts

### Data Loading
- Reading JSON files using Python’s built-in `json` module
- Printing raw data for inspection

### Data Cleaning
- Converting text ratings such as `"four"` or `"five"` into numeric values
- Handling missing ages by assigning `None`
- Removing duplicate customer records

### Data Analysis
- Calculating the **average customer rating**
- Identifying **poor ratings** (ratings < 3)
- Computing the **percentage of poor ratings**

### Recommendation Logic
- Ratings **≥ 4** → Recommend **Apple**
- Ratings **< 4** → Recommend **Samsung**

---

## Usage Examples

### Loading JSON Data
```python
import json

with open("store_data.json", "r") as file:
    data = json.load(file)
    print(data)
````

### Converting Text Ratings to Numbers

```python
rating_map = {
    "one": 1,
    "two": 2,
    "three": 3,
    "four": 4,
    "five": 5
}

if isinstance(rating, str):
    rating = rating_map.get(rating.lower())
```

### Calculating Average Rating

```python
average_rating = sum(ratings) / len(ratings)
print("Average rating:", average_rating)
```

---

## Sample Cleaned Data Output

```text
Name: Alice
Rating: 5
Age: 25

Name: Charlie
Rating: 2
Age: None
```

---

## Insights Example

From sample execution:

* **Average Rating:** 3.9
* **Poor Ratings (< 3):** 20% of users
* **Recommendations:**

  * High ratings favor **Apple**
  * Lower ratings favor **Samsung**

-

## Learning Outcomes

After completing this project, you will understand:

* ✓ How to load and parse JSON data in Python
* ✓ Techniques for cleaning inconsistent datasets
* ✓ Handling missing and duplicate values
* ✓ Calculating basic statistics from real-world data
* ✓ Implementing rule-based recommendation logic
* ✓ Working with Jupyter Notebooks for data analysis

---

## File Structure

```
Amazon-Store-Data/
├── README.md
├── Amazon-Store-data.ipynb
└── store_data.json
```

-

## Requirements

* Python 3.x
* Jupyter Notebook
* No external libraries required (uses built-in modules)

-

## Getting Started

1. Clone or download this repository
2. Ensure `store_data.json` is in the same directory as the notebook
3. Open the notebook:

   ```bash
   jupyter notebook Amazon-Store-data.ipynb
   ```
4. Run the cells sequentially to view results

-

## Topics Covered

* JSON Data Handling
* Data Cleaning Techniques
* Missing Value Handling
* Duplicate Removal
* Basic Statistical Analysis
* Rule-Based Recommendations
* Python Data Analysis Basics

-

## Notes

* The dataset is intentionally small for learning purposes
* Text and numeric ratings are mixed to simulate real-world data
* The project is suitable for beginners in Python and data analysis

---

**Last Updated**: January 2026


