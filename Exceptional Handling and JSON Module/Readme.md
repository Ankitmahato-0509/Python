## Amazon Store Data Analysis
-- A practical Python project demonstrating data cleaning, analysis, and basic recommendation logic using customer review data stored in JSON format.

## Overview
-- This repository contains a Jupyter notebook and a sample JSON dataset used to analyze customer feedback from an Amazon-like online store.
-- The project focuses on:
-- Cleaning inconsistent real-world data
-- Handling missing and duplicate values
-- Deriving meaningful insights from customer ratings
-- Generating simple brand recommendations

## Contents
-- Main project files included in this repository

## Main Files
-- Amazon-Store-data.ipynb
-- Jupyter notebook with step-by-step data analysis
-- Loads JSON data using Python’s json module
-- Cleans inconsistent ratings (text to numeric)
-- Handles missing values (e.g., age)
-- Removes duplicate customer entries
-- Computes statistics and generates recommendations

-- store_data.json
-- Sample JSON dataset with 6 customer reviews
-- Fields included:
-- name – Customer name
-- rating – Numeric or text-based rating
-- feedback – Customer feedback text
-- age – Customer age (some values missing)

## Key Concepts
-- Core ideas demonstrated in the project

## Data Loading
-- Reading JSON files using Python’s built-in json module
-- Printing raw data for inspection

## Data Cleaning
-- Converting text ratings such as "four" or "five" into numeric values
-- Handling missing ages by assigning None
-- Removing duplicate customer records

## Data Analysis
-- Calculating the average customer rating
-- Identifying poor ratings (ratings < 3)
-- Computing the percentage of poor ratings

## Recommendation Logic
-- Ratings ≥ 4 recommend Apple
-- Ratings < 4 recommend Samsung

## Usage Examples
-- Common operations demonstrated in the notebook

## Loading JSON Data
```python
import json
with open("store_data.json", "r") as file:
    data = json.load(file)
    print(data)
