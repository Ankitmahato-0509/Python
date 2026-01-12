Amazon Store Data Analysis
This repository contains a Jupyter notebook and sample JSON dataset for analyzing customer feedback from an Amazon-like store. The notebook loads, cleans, and derives insights from the data, including average ratings and recommendations.
​

Files
store_data.json: JSON array with 6 customer reviews, including fields for name, rating (text or numeric), feedback, and age (some missing).
​

Amazon-Store-data.ipynb: Python notebook using json library to load data, clean inconsistencies (e.g., text ratings to numbers, duplicates), compute stats like average rating (3.9) and poor rating percentage (20%), and generate brand recommendations.
​

Setup
Ensure Python 3 and Jupyter are installed.

Place store_data.json in the same directory as the notebook.

Open Amazon-Store-data.ipynb in Jupyter and run cells sequentially.

Usage
Run the notebook to:

Load and print raw data.

Clean: Convert text ratings (e.g., "four" to 4), handle missing ages, remove duplicates.

Generate insights: Average rating, poor rating percentage.

Produce recommendations: Suggest "Apple" for high ratings (≥4), "Samsung" otherwise.
​

Example cleaned data output includes entries like Alice (rating 5, age 25) and Charlie (rating 2, age None).
​

Insights Example
From sample execution:

Average rating: 3.9

20% users with poor rating (<3)

Recommendations favor Apple for top reviewers
