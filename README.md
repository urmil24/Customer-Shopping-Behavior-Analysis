# Customer-Shopping-Behavior-Analysis
This project analyzes 3,900+ customer shopping records using Python, SQL, and Power BI to uncover spending patterns, product trends, and customer behavior. The insights help businesses improve marketing, boost revenue, and make data-driven decisions.

# Customer Shopping Behavior Analysis

A Data Analytics project using Python, PostgreSQL (SQL), and Power BI to understand customer behavior, spending patterns, product trends, and business insights from 3,900+ shopping transactions.

# Project Overview

This project analyzes detailed shopping behavior data consisting of 3,900 purchase records across 18 features.

The objective is to extract actionable insights for improving customer retention, product strategies, and revenue growth.

The workflow includes:
✔ Cleaning and processing data using Python
✔ Advanced business analysis using SQL
✔ Interactive insight visualization using Power BI
✔ Deriving business recommendations based on the findings

# Dataset Summary

Rows: 3,900

Columns: 18

Key Features Include:

Demographics: age, gender, location, subscription status

Purchase Details: item purchased, category, purchase amount, season

Product Attributes: size, color

Customer Behavior: discount applied, promo code used, review rating

Others: previous purchases, frequency, shipping type

#  Missing Values:

37 missing values in review_rating, imputed using category-wise median.

🧹 Data Preprocessing (Python)
✔ Steps Performed

Data Loading: Imported using pandas

EDA:

df.info(), df.describe(), value counts

Missing Data Imputation:

Filled missing ratings using median per product category

Column Name Standardization:

Converted column names to snake_case

Feature Engineering:

age_group (binned age into categories)

purchase_frequency_days (calculated from timestamps)

Data Consistency Checks:

Removed redundant promo_code_used if discount already applied

Database Integration:

Inserted cleaned data into PostgreSQL for SQL querying

# Business Analysis Using SQL (PostgreSQL)

A series of 10 analytical SQL queries were executed to derive insights:

Revenue by Gender – Who spends more?

High-Spending Discount Users – Customers who use discounts yet spend more than average

Top 5 Highest-Rated Products

Standard vs Express Shipping – Which group spends more?

Subscribers vs Non-Subscribers – Revenue and average order value comparison

Discount-Dependent Products – Products frequently bought on discount

Customer Segmentation – New vs Returning vs Loyal customers

Top 3 Products Per Category

Repeat Buyers & Subscription Trend – Do repeat purchasers subscribe more?

Revenue by Age Group

# Power BI Dashboard

An interactive dashboard was created to visualize:

Overall revenue and order trends

Customer demographics

Seasonal demand patterns

Product category performance

Subscription impact

High-value customers

Ratings and satisfaction metrics

The dashboard helps stakeholders quickly understand business patterns and make data-driven decisions.

#  Business Recommendations

Based on the analysis:

📍 1. Promote Subscription Benefits

Subscribers spend more—offer exclusive rewards and discounts.

📍 2. Strengthen Loyalty Programs

Encourage repeat purchases with reward points, special offers, and personalized deals.

📍 3. Optimize Discounts

Identify products overly dependent on discounts and adjust pricing strategies.

📍 4. Utilize Top-Rated Products

Use high-rated items in marketing campaigns to increase conversion.

📍 5. Target High-Value Segments

Focus on:

High-spending age groups

Express shipping users

Loyal customers

# Tech Stack
Technology	Purpose
Python (Pandas, NumPy, Matplotlib)	Data cleaning & EDA
PostgreSQL	SQL-based business analysis
Power BI	Interactive dashboards
Jupyter Notebook	Analysis workflows
