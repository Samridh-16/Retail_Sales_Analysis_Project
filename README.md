# Retail Sales Performance Analysis

## Overview

This project analyzes a **Retail Sales dataset** sourced from Kaggle to evaluate business performance across revenue trends, product performance, customer behavior, and profitability.

The objective is to simulate a real-world retail analytics workflow using Python, SQL, and Power BI to generate actionable business insights.

---

## Tech Stack

- **Python (Pandas)** – Data cleaning & feature engineering
- **SQL (MySQL / BigQuery syntax)** – Business-driven data analysis
- **Power BI** – Interactive dashboard development

---

## Dataset Source

### Retail Sales Dataset (Kaggle)

[https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset](https://www.kaggle.com/datasets/mohammadtalib786/retail-sales-dataset)

---

## Repository Structure

### 📊 Dashboard

Contains Power BI dashboard screenshots highlighting revenue, customer, and profitability insights.

### 📁 Dataset

Includes:

- Raw dataset
- Cleaned dataset used for SQL and visualization

### 🐍 Python

Contains the data cleaning and preprocessing script used to:

- Create derived time variables
- Calculate profit and margin
- Engineer analytical features

### 📝 SQL Query

Business-oriented SQL queries designed to answer key analytical questions such as revenue trends, customer segmentation, and seasonal performance.

### 📈 SQL Query Results

Outputs from executed queries used to validate KPIs and dashboard metrics.

---

## Cleaned Dataset – Data Dictionary

| Column Name | Description |
|---|---|
| transaction_id | Unique transaction identifier |
| date | Transaction date |
| customer_id | Unique customer identifier |
| gender | Customer gender |
| age | Customer age (numeric) |
| age_group | Categorized age segment |
| product_category | Product category (Beauty, Clothing, Electronics) |
| quantity | Units purchased |
| price_per_unit | Selling price per unit |
| unit_cost | Cost per unit |
| total_amount | quantity × price_per_unit |
| revenue | Transaction revenue |
| total_cost | quantity × unit_cost |
| profit | revenue − total_cost |
| profit_margin | profit ÷ revenue |
| year | Extracted year |
| quarter | Extracted quarter |
| month | Numeric month |
| month_name | Month name |
| day_of_week | Day of week |
| is_weekend | Weekend indicator |

---

## Analytical Scope

This project includes:

- Monthly and quarterly revenue analysis
- Year-over-Year growth calculation
- Profitability by category
- Weekend vs Weekday performance
- RFM-based customer segmentation
- Seasonal performance index
- Top-performing products by quarter

---

## Key Business Objective

To identify **revenue drivers**, **seasonal patterns**, and **customer segmentation opportunities** that can improve retention and profitability in a retail environment.
