
# Advanced-SQL-with-Ecommerce-Data
Advanced SQL with Transaction Level Ecommerce Data for Google BigQuery 


This document provides an overview of a comprehensive SQL script designed for Google BigQuery. This script transforms and analyzes customer, product, and transaction data to extract meaningful insights and support data-driven decision-making.

## Description

The Master BigQuery Script includes data importation, data exploration, customer segmentation, and advanced analytics. Developed initially in SQL Server and VS Code, it was adapted for BigQuery to leverage Google Cloud's analytics capabilities. The script operates on manually loaded CSV files (customers, products, and transactions) into your custom dataset and generates a series of analytical tables providing insights into customer behavior, sales trends, and product performance.

### Key Features

- **Data Integration**: Combines data from multiple sources into a unified view, enabling comprehensive analysis.
- **Data Exploration**: Analyzes total transactions and revenue by product category, identifies top revenue-generating users, and assesses revenue differences between weekdays and weekends.
- **Customer Segmentation**: Categorizes customers into segments such as One-Time Buyers, Frequent Buyers, and High-Value Customers to tailor marketing and sales strategies.
- **Advanced Analytics**: Calculates average, median, and 90th percentile purchase amounts, performs a 7-day rolling average of daily revenue, and determines week-over-week percentage changes in weekly revenue.
- **Product Recommendations**: Generates personalized product recommendations for each customer based on purchase history.
- **Customer Preferred Shopping Seasons**: Identifies each customer's preferred shopping seasons, enhancing seasonal marketing efforts.
- **Cohort Analysis**: Measures cohort lifetime value and average first-month revenue to assess customer value over time.

### Implementation Details

1. **Core Data Staging**: Merges transaction, customer, and product data into a staging table for further analysis.
2. **Total Transactions and Revenue by Category**: Aggregates total number of transactions and total revenue by product category.
3. **Top 10 Users by Revenue**: Identifies the top 10 customers by total revenue generated.
4. **Weekday vs. Weekend Revenue Analysis**: Calculates average revenue differences between weekdays and weekends.
5. **Customer Segmentation Tables**: Creates tables for each customer segment based on purchase behavior and spending patterns.
6. **Advanced Analytics Tables**:
   - Calculates a 7-day rolling average of daily revenue.
   - Determines average revenue across different time periods (weekend/weekday, day of the week, and by retail season).
   - Computes average, median, and 90th percentile purchase amounts.
7. **Product Recommendations by Customer**: Uses product pairing to recommend products to customers based on their purchase history.
8. **Cohort Analysis**: Analyzes cohorts based on first purchase date to determine lifetime value and first-month revenue.

## Usage

This script is intended to run as a one-time setup. It supports a wide range of analytical and business intelligence applications, from customer behavior analysis to financial forecasting and strategic planning.

## Requirements

- Google BigQuery: The script is designed for Google BigQuery and requires an active Google Cloud project with BigQuery enabled.
- Dataset Preparation: Customers, products, and transactions data must be manually loaded into the your custom dataset within BigQuery.

## Contributions

While the script has been thoroughly tested, contributions, suggestions, and improvements are welcome. Please report any issues or bugs encountered during implementation.


