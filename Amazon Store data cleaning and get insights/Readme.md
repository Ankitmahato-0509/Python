Amazon Store Data Analysis

This project analyzes customer feedback data from an Amazon-like online store using Python and Jupyter Notebook. It focuses on cleaning inconsistent data, deriving meaningful insights from customer reviews, and generating simple brand recommendations based on ratings.

📁 Project Structure
├── store_data.json
├── Amazon-Store-data.ipynb
└── README.md

Files Description

store_data.json
A JSON array containing 6 customer reviews with the following fields:

name – Customer name

rating – Rating (numeric or text, e.g., "four")

feedback – Customer review text

age – Customer age (some values missing)

Amazon-Store-data.ipynb
A Jupyter Notebook that:

Loads the JSON data

Cleans and standardizes ratings

Handles missing values and duplicates

Computes key statistics

Generates brand recommendations

⚙️ Setup Instructions

Ensure Python 3 and Jupyter Notebook are installed.

Place store_data.json in the same directory as the notebook.

Open the notebook:

jupyter notebook Amazon-Store-data.ipynb


Run the cells sequentially.

🚀 Usage

When you run the notebook, it will:

Load and display raw data

Clean the dataset

Convert text ratings (e.g., "four" → 4)

Handle missing age values

Remove duplicate entries

Generate insights

Average customer rating

Percentage of poor ratings

Produce recommendations

Recommend Apple for users with ratings ≥ 4

Recommend Samsung for users with ratings < 4

🧹 Example Cleaned Data
Name: Alice
Rating: 5
Age: 25

Name: Charlie
Rating: 2
Age: None

📊 Insights (Sample Output)

Average Rating: 3.9

Poor Ratings (< 3): 20% of users

Recommendation Trend:

High-rating users → Apple

Lower-rating users → Samsung
