# Retail Sales Analysis | SQL + Power BI

## Overview
This project analyzes retail sales data to uncover trends in revenue, product performance, and customer behavior. I used T-SQL to clean and prepare the raw data, then built an interactive Power BI dashboard to visualize the results.

## What I Did
- Reviewed the business request and user stories to understand what questions the dashboard needed to answer
- Identified the relevant FACT and DIMENSION tables from the source database
- Wrote T-SQL queries to clean, filter, and transform the data — including column renaming, string functions, CASE statements, NULL handling, and multi-table joins
- Extended the base queries to capture additional fields for deeper analysis:
  - Added **Yearly Income** to the customer table to enable income-based segmentation
  - Added **List Price** to the product table to support pricing/category analysis
  - Added **Week Number** to the date table for weekly (not just monthly) trend analysis
  - Added **Order Quantity** to the sales fact table to analyze units sold, not just revenue
- Exported cleaned tables and loaded them into Power BI
- Built a relational data model connecting Customer, Product, Calendar, and Sales tables
- Created an interactive dashboard with bar charts, line charts, a map visual, and top-10 rankings

## Tools Used
SQL Server (T-SQL), Power BI Desktop

## Key Concepts Applied
- Star schema design (FACT vs. DIMENSION tables)
- Table joins (LEFT JOIN across multiple related tables)
- Data cleaning: CASE statements, ISNULL, string functions
- Dynamic vs. static date filtering
- Power BI data modeling and dashboard design

## Files in this Repo
- `DIM_Customer_Clean.sql`, `DIM_Product_Clean.sql`, `DIM_Calendar_Clean.sql`, `FACT_InternetSales_Clean.sql` — SQL scripts for data cleaning
- `*.csv` — exported cleaned datasets
- `Sales Report.pbix` — Power BI dashboard file
- `Sales Report.pdf` — static screenshot of the dashboard

## Dashboard
Download `Sales Report.pbix` from this repo and open in Power BI Desktop for the interactive version, or view `Sales Report.pdf` for a static screenshot.
