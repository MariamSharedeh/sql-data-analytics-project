#  SQL Data Analytics Project

A comprehensive collection of **SQL scripts** for data exploration, analytics, and reporting.

This repository contains a variety of SQL queries designed to  **data analysts** and **BI professionals** quickly explore, segment, and analyze data within a relational database.

---

## Project Overview

## 🗂️ SQL Script Descriptions

| File | Description |
|------|--------------|
| `init_database.sql` | Initializes the demo database with sample tables and data for testing all analyses. |
| `database_exploration.sql` | Explores database structure: tables, columns, and basic statistics. |
| `dimensions_exploration.sql` | Lists categorical dimensions and explores their distinct values. |
| `date_range_exploration.sql` | Analyzes date distributions, min/max dates, and missing periods. |
| `measures_exploration.sql` | Studies numeric measures (min, max, avg, stddev, null count). |
| `magnitude_analysis.sql` | Evaluates the relative magnitude (size, importance) of different metrics. |
| `part_to_whole_analysis.sql` | Calculates ratios and percentage contributions (e.g., sales share per region). |
| `change_over_time_analysis.sql` | Measures time-based variations (month-over-month, year-over-year). |
| `cumulative_analysis.sql` | Computes running totals and moving averages using window functions. |
| `data_segmentation.sql` | Groups data into meaningful segments (customer types, sales ranges, etc.). |
| `performance_analysis.sql` | Tracks KPIs and compares performance between periods or groups. |
| `ranking_analysis.sql` | Ranks entities (top products, top customers, etc.) using RANK/DENSE_RANK. |
| `report_customers.sql` | Generates a summarized report of customer activity and metrics. |
| `report_products.sql` | Creates an aggregated report of product-level performance and trends. |

---

##  How to Use

1. Run `init_database.sql` to set up the base schema and data.  
2. Execute any of the analysis scripts to explore or visualize different analytical views.  
3. Each script can be run independently and modified for your own dataset.

---

##  Example

```sql
SELECT 
    MIN(order_date) AS first_order_date,
    MAX(order_date) AS last_order_date,
    DATEDIFF(MONTH, MIN(order_date), MAX(order_date)) AS order_range_months
FROM gold.fact_sales;


Each SQL script focuses on a specific analytical theme and demonstrates **best practices** for:
- Clean, readable SQL  
- Efficient query design  
- Use of window functions, CTEs, and joins  
- Proper use of indexes and filtering  

---



 Author
Mariam Sharedeh
 Passionate about Data Analytics, SQL, and Business Intelligence

