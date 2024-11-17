
# Sales Analysis Project
## Overview
This project performs a comprehensive sales analysis by leveraging SQL, Excel, and Power BI. It covers customer records, transactions, revenue generation, and market-specific insights. The analysis focuses on critical dimensions such as time (year, month), markets, and currency. Visualizations are created using Power BI to provide an interactive and insightful representation of the data.

# Key Features
Customer Insights:

Display all customer records.

Count the total number of customers.

Market-Specific Analysis:

Analyze transactions specific to markets, such as Chennai (Market Code: Mark001).

Identify products sold in specific markets.

Currency-Based Analysis:

Filter transactions based on currency (e.g., USD, INR).

# Time-Specific Analysis:

Aggregate transactions by year, month, and other time-based filters.

Focus on yearly revenue and market-specific revenue.

# Interactive Dashboards:

Visualize sales data with Power BI for better insights and decision-making.

# Tools and Technologies

# SQL:

Used for querying and analyzing transactional data.

Joins and aggregations to extract actionable insights.

# Excel:

Data cleaning and exploratory analysis.

Summary tables and pivot charts for quick insights.

# Power BI:
Created visualizations and dashboards for dynamic analysis.

Highlighted key performance indicators (KPIs) such as revenue and customer metrics.

Data Analysis Using Power BI
============================

1. Formula to create norm_amount column

`= Table.AddColumn(#"Filtered Rows", "norm_amount", each if [currency] = "USD" or [currency] ="USD#(cr)" then [sales_amount]*75 else [sales_amount], type any)`



