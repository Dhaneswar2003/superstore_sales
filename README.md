# Superstore_sales
Python cleans and processes the Superstore dataset, SQL creates analytical summary tables, and Tableau Public is used to build an interactive sales dashboard.

# Project Overview
This project demonstrates a complete end-to-end data analysis pipeline using the Superstore sales dataset.
The workflow includes:
Python → Data cleaning, preprocessing, transformation
SQL → Creation of analytical summary tables
Tableau Public → Interactive dashboard for visualization
This project showcases practical skills used in real-world data analytics: ETL, data modeling, SQL summarization, and BI dashboard development.

# Python – Data Cleaning & Preprocessing
Python was used as the primary tool for preparing the dataset before analysis.
Key Steps Performed
Removed unnecessary columns
Dropped duplicate rows
Handled missing/null values
Converted date formats
Standardized column types
Added new fields (Year, Month, Month Name) for time-series analysis
Exported cleaned dataset for SQL & Tableau
# Output File
clean_superstore.csv

# SQL – Analytical Summary Table Creation
SQL was used to convert the cleaned dataset into structured analytical tables.
Summary Tables Generated
# Table Name	               Description
total_sales	               Overall sales value
sales_by_category	         Sales grouped by product category
sales_by_region	           Regional sales performance
sales_by_segment	         Sales by customer segment
monthly_sales_trend	       Year–month sales time series
top_10_products	           Best-selling products
shipping_time_analysis	   Average shipping days per ship mode

These tables were exported for visualization in Tableau Public.

# Tableau Public – Dashboard Creation
The cleaned dataset and SQL summary tables were uploaded to Tableau Public to build an interactive dashboard.
Dashboard Includes:
* Total Sales KPI
* Sales by Category
* Sales by Region (Map)
* Sales by Customer Segment
* Monthly Sales Trend (Line Chart)
* Top 10 Products
* Shipping Time Analysis
* Custom filters for interactive exploration

# Project Architecture
superstore-sales-analysis/

data/
-superstore_sales_dataset.csv
-clean_superstore.csv
-sales_by_category.csv
-sales_by_segment.csv
-sales_by_region.csv
-monthly_sales.csv
-top_10_products.csv
-shipping_time.csv

python/
-cleaning_and_processing.ipynb

sql/
-summary_tables.sql

tableau/
-dashboard.twbx(optional)
-README.md

# How to Run This Project

Step 1 — Run Python Script
python clean_superstore.py

Step 2 — Open SQL Tool (MySQL / SQLite)
Run the summary_tables.sql script to create all summary tables.

Step 3 — Upload CSV Files to Tableau Public
* Create a new workbook
* Upload all summary CSV files
* Build worksheets for each metric
* Combine them into a dashboard

# Tech Stack Used
* Python → Pandas, NumPy
* SQL → SQLite / MySQL
* Tableau Public → Dashboard & data storytelling
* GitHub → Project Documentation
