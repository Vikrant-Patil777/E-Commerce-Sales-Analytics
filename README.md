# 📊 E-Commerce Sales Analytics

# Project Overview

This project follows an end-to-end data analytics workflow:

**Original Dataset → Excel Data Cleaning → SQL Analysis → Python (Pandas) EDA → Power BI Dashboard**

The objective is to transform raw e-commerce sales data into meaningful business insights that help understand sales performance, profitability, customer behavior, product performance, and regional trends.

# Dataset

**Global E-Commerce Sales Dataset (2021–2024) — Kaggle**

- Total Records: 10,000
- Total Columns: 23
- Data Type: Structured e-commerce sales data

The dataset contains information about orders, customers, products, categories, regions, revenue, cost, profit, discounts, shipping, and payment methods.

# Objectives

- Analyze overall e-commerce sales performance.
- Measure total revenue and profit.
- Understand monthly and yearly sales trends.
- Identify top-performing products and categories.
- Analyze regional sales performance.
- Understand customer segment contribution.
- Examine order status distribution.
- Perform Exploratory Data Analysis (EDA) using Python.
- Build an interactive sales dashboard in Power BI.

# Tools & Technologies

| **Tool** | **Purpose** |
|---|---|
| **Microsoft Excel** | Dataset storage, data cleaning, and preparation |
| **MySQL** | SQL queries and business-question analysis |
| **Python (Pandas)** | Exploratory Data Analysis (EDA) |
| **Power BI** | Data modeling, DAX calculations, visualization, and dashboard development |
| **GitHub** | Project documentation and portfolio presentation |

# Data Cleaning — Excel

The original dataset was reviewed and prepared before analysis. The cleaned dataset is maintained separately from the original dataset to keep the transformation process traceable.

Data cleaning activities include:

- Checked missing values.
- Checked duplicate records and Order IDs.
- Corrected inconsistent order status values.
- Reviewed column names and data formats.
- Verified numerical values.
- Checked revenue, cost, profit, and profit margin calculations.
- Prepared the cleaned dataset for further analysis.

**Data Cleaning Workflow**

Original Dataset  
↓  
Data Inspection  
↓  
Data Cleaning  
↓  
Cleaned Dataset

# SQL Analysis — MySQL

SQL was used to analyze the e-commerce dataset and answer important business questions.

The analysis includes:

- Overall sales and profit analysis.
- Yearly revenue and profit analysis.
- Monthly sales trends.
- Revenue and profit by category.
- Revenue and profit by region.
- Top 10 products by revenue.
- Top 10 products by profit.
- Revenue and profit by customer segment.
- Top 10 customers by revenue.
- Discount and profit analysis.
- Order status analysis.
- Shipping method analysis.
- Payment method analysis.
- Seasonal performance.
- Profit margin by category.

**SQL Techniques Used**

- SELECT
- DISTINCT
- WHERE
- GROUP BY
- ORDER BY
- HAVING
- Aggregate Functions
- JOIN
- CASE
- Date Functions
- Subqueries

# Exploratory Data Analysis (EDA) — Python (Pandas)

Python Pandas was used to perform Exploratory Data Analysis and understand the dataset before dashboard development.

### Data Understanding

- Loaded the cleaned CSV dataset using Pandas.
- Viewed the first five records.
- Checked dataset dimensions.
- Examined column names.
- Checked data types.
- Generated statistical summaries.

### Data Quality

- Checked missing values.
- Checked duplicate records.
- Checked duplicate Order IDs.
- Converted Order Date into datetime format.

### Numerical Analysis

- Total Revenue.
- Total Profit.
- Average Order Value (AOV).
- Total Quantity Sold.
- Average Discount.
- Overall Profit Margin.

### Business Analysis

- Revenue and Profit by Category.
- Revenue and Profit by Region.
- Top 10 Products by Revenue.
- Revenue by Customer Segment.
- Order Status Analysis.
- Monthly Revenue Trend.
- Yearly Revenue Trend.

**Pandas Functions Used**

- read_csv()
- head()
- shape
- info()
- describe()
- isnull()
- duplicated()
- sum()
- mean()
- groupby()
- sort_values()
- value_counts()
- to_datetime()

# Power BI Dashboard

The cleaned dataset and analysis were used to develop an interactive **E-Commerce Sales Analytics Dashboard** in Power BI.

### Data Modeling

- Created dimension tables from the main sales table.
- Established relationships between fact and dimension tables.
- Created a date dimension table.
- Implemented one-to-many relationships.

### DAX Measures

Created measures to calculate:

- Total Revenue
- Total Profit
- Total Orders
- Total Quantity
- Profit Margin

### Dashboard KPIs

- Total Revenue
- Total Profit
- Total Orders
- Total Quantity
- Profit Margin

### Dashboard Visualizations

- Monthly Revenue and Profit Trend.
- Revenue and Profit by Category.
- Revenue by Region.
- Revenue by Customer Segment.
- Top 5 Products by Revenue.

### Interactive Filters

- Year
- Region
- Category
- Order Status

The interactive dashboard allows users to explore sales performance and compare business results across different dimensions.

# Key Business Questions

This project addresses important business questions such as:

1. What is the total revenue and profit generated by the company?
2. How many unique orders were placed?
3. What is the average order value?
4. How do revenue and profit change yearly?
5. Which product categories generate the highest revenue and profit?
6. Which regions contribute the most to overall revenue?
7. Which products are the top revenue generators?
8. Which customer segments contribute the highest revenue?
9. What is the distribution of delivered, returned, processing, and cancelled orders?
10. How does revenue change across different months?
11. Which seasons perform best in terms of sales?
12. Which shipping and payment methods are commonly used?

# Business Recommendations

Based on the analysis, businesses can consider the following recommendations:

- **Improve Product Performance:** Focus on high-performing products and review the performance of low-revenue products.
- **Increase Profitability:** Monitor product costs and discount strategies to improve profit margins.
- **Regional Growth:** Identify strong-performing regions and explore opportunities to improve sales in lower-performing regions.
- **Customer Segmentation:** Develop targeted marketing strategies for different customer segments.
- **Order Management:** Monitor returned and cancelled orders to identify opportunities to improve order completion.
- **Sales Planning:** Use monthly and seasonal sales trends to plan inventory and marketing campaigns.
- **Business Monitoring:** Use the Power BI dashboard to regularly track sales, profit, orders, and other important business indicators.

# Key Skills Demonstrated

This project demonstrates practical skills in:

- Data Cleaning and Preparation
- Excel
- SQL Querying
- Exploratory Data Analysis (EDA)
- Python and Pandas
- Data Modeling
- DAX Calculations
- KPI Development
- Interactive Dashboard Development
- Data Visualization
- Business Analysis
- Data-Driven Decision Making

# Author

**Vikrant Patil**  
Aspiring Data Analyst | Business Analyst

**Technical Skills:** Excel | SQL | Power BI | Python | Pandas
