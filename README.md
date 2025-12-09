📖 Overview

This project is an end-to-end data analytics study of 3,900 customer transactions. The goal was to identify key drivers of revenue, customer loyalty, and product performance. By building a data pipeline from Python to PostgreSQL, this project simulates a real-world business intelligence workflow to provide actionable recommendations for marketing and inventory strategies.

💾 Dataset

The analysis uses a transactional dataset comprising 3,900 rows and 18 columns.

Demographics: Age, Gender, Location, Subscription Status.

Purchase Details: Item Purchased, Category, Purchase Amount (USD), Size, Color, Season.

Behavioral Metrics: Review Rating, Shipping Type, Discount Applied, Previous Purchases, Frequency of Purchases.

Data Preparation:

Standardized all 18 column names to snake_case for database consistency.

Imputed 37 missing values in the Review Rating column using category-specific medians.

🛠️ Tools Used

Python (Pandas, NumPy): For data extraction, cleaning, handling missing values, and feature engineering.

PostgreSQL: For structured data storage and complex business logic queries.

Power BI: For creating an interactive dashboard to visualize trends.

🔄 Project Steps

1. Data Cleaning & Engineering (Python)
Ingestion: Loaded raw CSV data using Pandas.

Transformation:

Created an age_group column to segment customers (e.g., Adults, Seniors).

Derived purchase_frequency_days to analyze engagement intervals.

Removed redundant columns (e.g., Promo Code Used) to ensure 3NF (Third Normal Form) compliance.

Loading: Connected Python to PostgreSQL to export the clean dataset.

2. Business Analysis (SQL)
Executed 10 key business queries in PostgreSQL, including:

Revenue Optimization: Comparing revenue contribution by Gender and Age Group.

Customer Segmentation: Categorizing users into New, Returning, and Loyal segments based on purchase history.

Operations Analysis: Evaluating if "Express" shipping correlates with higher cart values.

Product Performance: Identifying the top 3 best-selling products per category.

3. Visualization & Reporting (Power BI)
Developed an interactive dashboard to visualize:

Sales distribution across different seasons.

The correlation between Subscription Status and Total Spend.

Top-rated products to prioritize in marketing campaigns.

Dashboard

<img width="995" height="528" alt="image" src="https://github.com/user-attachments/assets/c8580b36-aa16-4571-b867-05d426b72735" />
The dashboard highlights that subscribers have a significantly higher retention rate and that specific product categories drive the majority of seasonal revenue.

📈 Key Results

Subscriber Value: Subscribers consistently show a higher average transaction value than non-subscribers.

Loyalty: A distinct segment of "Returning" customers was identified as a prime target for loyalty programs.

Shipping Trends: Customers opting for Express Shipping tend to have higher basket sizes.
