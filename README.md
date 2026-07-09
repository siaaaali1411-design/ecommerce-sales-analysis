# E-commerce Sales Analysis

## Project Overview

This project analyzes online retail transaction data to explore sales performance, customer behavior, and market distribution.

The project combines Python data analysis and MySQL database analysis to build an end-to-end data analysis workflow.

---

## Dataset

Dataset: Online Retail Dataset

- Approximately 400,000 transaction records
- Transaction information including:
  - InvoiceNo
  - Product
  - Quantity
  - Unit Price
  - Customer ID
  - Country
  - Invoice Date

---

## Tools & Technologies

- Python
  - Pandas
  - NumPy
  - Matplotlib

- Database
  - MySQL

- SQL Techniques
  - GROUP BY
  - Aggregate Functions
  - DATE_FORMAT
  - COUNT DISTINCT
  - Window Functions (RANK)

---

# Analysis Workflow

## 1. Data Cleaning (Python)

Used Pandas to preprocess raw transaction data:

- Removed missing customer records
- Removed invalid transactions
- Filtered abnormal quantity and price values
- Created sales metric:
Sales = Quantity × UnitPrice

---

# 2. Sales Analysis (Python + SQL)

## Top Products

Analyzed product sales contribution and identified best-selling products.

## Monthly Sales Trend

Explored revenue changes over time and identified seasonal sales peaks.

## Country Sales Analysis

Analyzed revenue contribution across different markets.

---

# 3. Customer Analysis

## RFM Customer Segmentation

Calculated:

- Recency
- Frequency
- Monetary

Segmented customers into:

- Champions
- Loyal Customers
- New Customers
- At Risk Customers


## High Value Customer Analysis

Used SQL aggregation to identify customers with high spending and frequent purchases.

---

# SQL Analysis

Implemented MySQL queries for:

- Product ranking
- Country revenue ranking
- Monthly revenue analysis
- Customer spending analysis
- Ranking analysis using window functions


SQL scripts:
sql/analysis.sql

---

# Visualization

## Sales Analysis

![Monthly Sales](images/monthly_sales.png)

![Top Products](images/top_products.png)

![Country Sales](images/country_sales.png)


## Customer Analysis

![Customer Segments](images/customer_segments.png)

![Revenue Distribution](images/customer_revenue_distribution.png)


---

# Key Insights

- United Kingdom contributed the majority of revenue.
- Sales increased significantly during September-November 2011.
- A small group of high-value customers contributed a large proportion of revenue.
- Customer segmentation helps identify loyal customers and potential churn risks.

---

# Future Improvements

- Build automated data pipeline
- Add interactive dashboard using Power BI/Tableau
- Apply machine learning models for customer prediction