# Tools Used: 
Excel · SQL (MySQL) · Power BI

Dataset: 1,200 e-commerce transaction records
Author: Akumah Esther Chinomso


# Project Overview

An end-to-end data analytics project analyzing e-commerce sales performance across 1,200 transactions.
The project covers the full analyst workflow from raw data cleaning through exploratory analysis, SQL querying, and final dashboard delivery.

- Key business findings:
- Total revenue of $1.26M across 1,200 orders
- 41.4% of orders were cancelled or returned a critical business risk
- Chairs and Printers were the top revenue generating product categories at $195.6k each
- Instagram drove the highest revenue of all referral channels
- Online was the most popular payment method
- Peak revenue month: June 2024 at $68,068


# Step 1 — Data Cleaning & Preparation

# Goal:
Clean the raw dataset by handling missing values, inconsistencies, duplicates, and incorrect data type formats.

# Process:
- Reviewed the full dataset before cleaning to understand structure and identify issues
- Duplicates: No duplicate Order IDs were found
- Missing values: The Coupon Code column had over 20% missing values — replaced with "No Coupon" to preserve row integrity
- Standardization: All categorical columns were trimmed and converted to Proper Case for consistency
Data types: All columns converted to correct formats (dates, numbers, text)
Currency formatting: Unit Price and Total Price formatted to USD ($) at 2 decimal places for accurate analysis

## Key Requirements
- Identify missing or null values
- Remove duplicates
- Correct data formats (dates, numbers, text)
- Trimmed the dataset
- Capitalized the categoryical data with Proper Case.

## Step by Step Data Cleaning
- Before I started cleaning the data, I looked through the dataset to understand what the dataset is all about, in the course of looking through the dataset, I saw some missing values, inconsistencies in some columns and inappropriate data type format. 
- I clean to ensure absolute accuracy in the dataset.
  
## Here is a breakdown of my data cleaning process:
- Handled Missing & Duplicate Data: No duplicate values were found in the Order ID while missing values in columns like Coupon codes column was replaced with "No Coupon" Because the missing values were over 20% values of the dataset.
- Standardized Format: AlL the inconsistencies in the Categorical columns were capitalized and trimmed.
- Number Formnats: I Changed all the columns into their proper data type format.
- Changed the Total price and Unit Price to Currency ($) to 2 decimal places for accurate trend analysis.

## Data Changes
- Original Dataset: 1,200 rows
- Cleaned Dataset: 1,200 rows
- Row Removed:No duplicate values found.
- Missing values: 309 null values was replaced with "No Coupon"
- Standardized Format: I Capitalized and trimmed all the Categorical columns
- Number Format: All columns were changed to its appropriate data type.

l am still learning and growing every day, but seeing raw, chaotic data transform into clear, actionable insights. Data cleaning leads to better insights.

# Result: 
Clean, analysis-ready dataset of 1,200 records.


# Step 2 — Exploratory Data Analysis (EDA)
 
## Goal
Analyze a dataset to understand patterns, 
trends, and distributions.
Identify and outliers using the Descriptive Statistics. 
My goal is to understand the data, find problems, and get ideas for what to analyze next.

## Key Requirements
- Calculate basic statistics (mean, median, count)
- Identify trends and outliers
- Summarize key observations

## Here's the outcome
- Using the standard Interquartile Range (IQR) rule, exactly 8 out of 1,200 transactions were flagged as statistical outliers (Threshold of Total Price > $3,330.41)
- Chairs ($195.6k) and Printers ($195.6k) represent the highest strategic cash flows, closely Followed by Laptops ($192.1k). Phone sales represent the lowest baseline performance channel ($151.7k) due to significantly suppressed market transaction volume (only 156 orders vs. the category mean of 172).
- Total Price Skewness = 0.89135 (Positive Skew) . The right tail is longer, most data clusters on the left. • Mean > Median > Mode. a
- Unit Price Skewness = -0.02651 (Approximately Symmetric) Extremely close to 0, indicating nearly perfect symmetry. - Mean = Median = Mode.
- Quantity Skewness = 0.027922 (Approximately Symmetric)
- Total Price Kurtosis = -0.040414 • Almost exactly 0. . The distribution is mesokurtic - very close to a normal distribution in terms of tail weight and outlier propensity.
- Unit Price Kurtosis = -1.19101 • Negative • Tails are much lighter than normal. · Distribution has fewer extreme outliers and a flatter peak (or a rounded, box-like shape) Compared to normal.
- Quantity Kurtosis (excess) = -1.29459 • Even more negative than 2. . Very light tails, very flat relative to normal. . Very low probability of extreme values.




# Step 3 — SQL Data Analysis (MySQL)

# Goal
Use SQL queries to extract insights from a dataset.
The project 3 is about Creating insights using SQL Queries 
(Clauses like: Select, From, Where, Group by and Order By) 
( Formulas like: Sum, Count and Avg) to extract Insights

# Setup
Created database: Decodelabs_Internship
Converted Excel file to CSV for import
Imported flat file: 14 columns, 1,200 rows

# Queries used: 
SELECT, FROM, WHERE, GROUP BY, ORDER BY, COUNT, SUM, AVG

## Key Requirements
- Write SELECT queries
- Use WHERE, ORDER BY, GROUP BY
- Perform aggregations (COUNT, SUM, AVG)

  ## Step by Step Procedures
  - I Created the Database and i named it Decodelabs_Internship.
  - I changed the Excel Xlxs to CSV (Comma Delimited).
  - I imported my flat file to the database I created.
  - Columns: 14
  - Rows: 1200

## Key Insights
- Revenue & Top Products
Total revenue: $1.26M across 1,200 orders
Chairs and Printers are the top revenue-generating product categories
- Cancellation & Return Rate — Critical Finding
497 out of 1,200 orders (41.4%) were either Cancelled or Returned
This is significantly high and indicates potential operational issues
Recommendation: Investigate which products have the highest cancellation and return rates. Review customer feedback to identify root causes and take corrective action.
- Marketing Channel Performance
Instagram drives the most revenue across all referral sources
Instagram and Facebook together account for 41.61% of total revenue
Recommendation: Prioritize social media advertising spend on Instagram and Facebook for maximum ROI
- Payment Method
Online is the most popular payment method across all transactions
  
## Experience
I encountered a lot of bugs while coding but was determined to handle it and boom! I did it after several trials.

## Files in this Repo
- select_queries.sql – Basic SELECT queries
- group_by_queries.sql – Grouping queries
- aggregations.sql – COUNT, SUM, AVG queries
- dataset.csv – Dataset used
- query_outputs.csv – Results

## Tools Used
- SQL, MySQL.


# Step 4 — Dashboard & Data Visualization

# Goal: 
Communicate insights clearly through charts and visual storytelling.
Charts created: Bar charts, pie charts, line charts.

# Dashboard Highlights
- Chairs ($195.6k) and Printers ($195.6k) represent the highest revenue categories
- Instagram and Facebook together drive 41.61% of revenue
41.4% of orders are lost to cancellations and returns — highest priority business issue
- Online is the dominant payment method
- Peak revenue: June 2024 — $68,068
  
# Skills Demonstrated
Data cleaning and preparation (Excel, Power Query)
Exploratory data analysis and descriptive statistics
Outlier detection using IQR method
SQL querying and database management (MySQL)
Data visualization and dashboard design (Excel, Power BI)
Business insight generation and recommendations



# About the Author
Akumah Esther Chinomso — Entry-level Data Analyst based in Port Harcourt, Nigeria.
Open to remote data analyst roles globally.
LinkedIn: linkedin.com/in/esther-akumah
GitHub: github.com/akumahesther Email: akumahesther@gmail.com





























 
