#Retail Sales Performance Analysis#
Introduction

This project presents a structured analysis of a Retail Sales dataset sourced from Kaggle. The objective is to evaluate business performance through multiple analytical perspectives, including revenue trends, product performance, customer purchasing behavior, and profitability analysis.

The project demonstrates how Python, SQL, and Power BI can be used together to transform raw transactional data into actionable business insights. The analysis focuses on identifying seasonal patterns, revenue drivers, customer segmentation patterns, and profit optimization opportunities.

This project is designed to reflect the practical workflow of a data analyst working in a retail business environment.

Tools and Technologies

Python (Pandas) – Data cleaning and preprocessing

SQL (MySQL / BigQuery syntax) – Business query analysis

Power BI – Dashboard visualization

Kaggle Retail Sales Dataset

Dataset Source

Retail Sales Dataset sourced from Kaggle:

https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset

Repository Structure Overview

This repository is organized into the following functional components:

Dashboard
Contains screenshots of the Power BI dashboard developed for revenue, profitability, and customer analysis.

Dataset
Includes both the original raw dataset and the cleaned dataset used for analysis and dashboard development.

Python
Contains the preprocessing script used to clean the dataset, create derived features (year, quarter, profit, margin), and prepare the dataset for SQL and Power BI analysis.

SQL Query
Contains structured SQL queries written to solve specific business problems such as revenue trends, customer segmentation, seasonal analysis, and profitability breakdown.

SQL Query Results
Contains the output results of executed SQL queries used to validate KPIs and dashboard metrics.

Cleaned Dataset – Data Dictionary

The cleaned dataset (retail_sales_cleaned.csv) contains the following variables:

transaction_id
Unique identifier assigned to each transaction.

date
Transaction date.

customer_id
Unique identifier for each customer.

gender
Customer gender.

age
Customer age in numeric format.

product_category
Category of the purchased product (Beauty, Clothing, Electronics).

quantity
Number of units purchased in the transaction.

price_per_unit
Selling price per unit.

total_amount
Total transaction amount calculated as quantity × price_per_unit.

year
Year extracted from the transaction date.

month
Numeric month value (1–12).

quarter
Quarter of the year (1–4).

day_of_week
Day of the week on which the transaction occurred.

month_name
Name of the month derived from the transaction date.

is_weekend
Boolean indicator identifying whether the transaction occurred on a weekend.

revenue
Revenue generated from the transaction.

unit_cost
Cost per unit of the product.

total_cost
Total cost calculated as quantity × unit_cost.

profit
Profit calculated as revenue minus total_cost.

profit_margin
Profit margin ratio calculated as profit divided by revenue.

age_group
Categorized age segment created for demographic analysis.

Analytical Scope

The analysis conducted in this project includes:

Monthly and quarterly revenue trend analysis

Year-over-Year growth evaluation

Profitability analysis by product category

Weekend versus weekday performance comparison

RFM-based customer segmentation

Seasonal sales performance analysis

Top-performing product analysis by quarter

Advanced SQL techniques used in the project include Common Table Expressions (CTEs), window functions (RANK, LAG, NTILE), moving averages, and revenue contribution calculations.
