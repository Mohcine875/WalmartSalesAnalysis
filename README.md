# Walmart Sales Analysis — SQL

## Project Overview

This project presents an end-to-end SQL analysis of Walmart sales transactions across three branches: Mandalay, Yangon, and Naypyitaw.

The objective is to analyze retail sales performance, customer behavior, product trends, revenue drivers, and branch-level performance using SQL. The project demonstrates how structured queries can transform raw transactional data into actionable business insights.

---

## Business Objectives

This analysis was designed to answer key business questions:

- Which branches generate the highest revenue?
- Which cities contribute the most to total sales?
- Which product lines perform best?
- What are the busiest sales periods?
- Which customer types generate the most revenue?
- Which payment methods are most commonly used?
- How do gender, city, and customer type affect sales performance?
- What patterns can be identified in revenue, quantity sold, gross income, VAT, and customer ratings?

---

## Dataset

The project uses a Walmart retail sales dataset containing more than 1,000 transactions across three branches.

| Property | Description |
|---|---|
| Dataset Type | Retail sales transactions |
| Rows | 1,000+ transactions |
| Branches | 3 branches |
| Cities | Mandalay, Yangon, Naypyitaw |
| Main Tool | SQL / MySQL |
| Source | Walmart sales dataset |

Main columns include:

- `invoice_id`
- `branch`
- `city`
- `customer_type`
- `gender`
- `product_line`
- `unit_price`
- `quantity`
- `tax_pct`
- `total`
- `date`
- `time`
- `payment`
- `cogs`
- `gross_margin_pct`
- `gross_income`
- `rating`

---

## Tools Used

| Tool | Purpose |
|---|---|
| SQL | Data querying and business analysis |
| MySQL | Database creation and query execution |
| CSV Dataset | Source data |
| GitHub | Project documentation and version control |

---

## Project Workflow

```text
Raw Sales Data
   ↓
Database Creation
   ↓
Data Wrangling
   ↓
Feature Engineering
   ↓
Exploratory SQL Analysis
   ↓
Business Insights
   ↓
Recommendations
```

---

## Database Setup

The SQL workflow starts by creating a dedicated database and a structured sales table.

Main setup steps include:

- creating the `walmartSales` database
- creating the `sales` table
- defining appropriate data types
- applying `NOT NULL` constraints
- setting `invoice_id` as the primary key
- importing the Walmart sales CSV file

This setup ensures the data is structured and ready for SQL-based analysis.

---

## Data Wrangling

The data wrangling phase focused on preparing the dataset for analysis.

Main steps included:

- reviewing the imported data
- validating table structure
- checking important fields
- preparing transaction data for aggregation
- ensuring each sale record is uniquely identified

---

## Feature Engineering

Three additional time-based features were created to support deeper analysis.

| Feature | Description |
|---|---|
| `time_of_day` | Groups transactions into Morning, Afternoon, and Evening |
| `day_name` | Extracts the day of the week from the transaction date |
| `month_name` | Extracts the month name from the transaction date |

These features help identify sales patterns by time of day, day of week, and month.

---

## Revenue and Profit Calculations

The analysis uses the following retail business calculations:

```text
COGS = unit_price × quantity
VAT = tax percentage applied to COGS
Total = COGS + VAT
Gross Income = Total − COGS
Gross Margin = Gross Income / Total Revenue
```

These calculations help evaluate revenue, cost, tax contribution, and profitability.

---

## SQL Analysis Areas

The project answers more than 20 business questions across three major analysis areas.

### Product Analysis

This section focuses on product-line performance.

Examples of questions answered:

- How many unique product lines are in the dataset?
- What is the most frequently sold product line?
- Which product line generated the highest revenue?
- Which product line generated the highest VAT?
- What is the average rating by product line?
- Which product lines performed above or below average?

### Sales Analysis

This section focuses on sales performance and revenue behavior.

Examples of questions answered:

- What is the total revenue by month?
- Which city generated the largest revenue?
- Which branch sold more products than average?
- Which time of day records the highest sales volume?
- Which customer type generates the most revenue?
- Which city has the highest average VAT percentage?

### Customer Analysis

This section focuses on customer behavior and segmentation.

Examples of questions answered:

- How many unique customer types are in the dataset?
- What is the most common customer type?
- What is the gender distribution across branches?
- Which payment method is most commonly used?
- Which time of day receives the highest average rating?
- Which day of the week has the best average customer rating?

---

## SQL Skills Demonstrated

This project demonstrates practical SQL skills including:

- database creation
- table creation with defined data types
- primary key usage
- data import preparation
- feature engineering with `ALTER TABLE` and `UPDATE`
- conditional logic using `CASE`
- aggregation using `SUM`, `AVG`, `COUNT`, `MIN`, and `MAX`
- grouping using `GROUP BY`
- filtering grouped results using `HAVING`
- sorting results with `ORDER BY`
- business KPI analysis using SQL queries

---

## Repository Contents

```text
WalmartSalesAnalysis/
│
├── README.md
├── SQL_queries.sql
└── WalmartSalesData.csv
```

> Note: The dataset filename in the repository may include extra characters depending on the uploaded file name.

---

## Key Findings

The SQL analysis identified several important insights:

- Food and Beverages generated the highest revenue overall.
- Evening hours consistently recorded the strongest sales activity.
- Female customers gave slightly higher ratings than male customers.
- Branch C, located in Naypyitaw, had the highest average customer rating.
- Customer type, payment method, and product line all influenced sales performance.
- Time-based analysis helped identify stronger sales periods during the day and week.
- Branch and city analysis helped compare store-level performance.

---

## Business Recommendations

Based on the analysis, the following actions are recommended:

- Prioritize inventory and promotions for top-performing product lines.
- Use evening sales patterns to optimize staffing and store operations.
- Monitor branch-level performance to identify best practices from high-performing locations.
- Use customer type and gender insights to improve targeted marketing campaigns.
- Track payment method preferences to improve checkout experience and customer convenience.
- Review lower-performing product lines to identify pricing, promotion, or placement opportunities.

---

## Project Value

This project demonstrates the ability to:

- build and query a SQL database
- clean and structure retail sales data
- engineer useful time-based features
- answer business questions using SQL
- analyze sales, customer, product, and branch performance
- extract business insights from transactional data
- communicate SQL analysis clearly in a professional portfolio project

---

## Technologies

- SQL
- MySQL
- CSV Data
- Data Wrangling
- Feature Engineering
- Retail Analytics
- Business Analytics
- GitHub

---

## Project Status

Completed as a SQL-based retail sales analysis project.

---

## Author

**Mohcine Behate**

SQL and Business Analytics Portfolio Project
