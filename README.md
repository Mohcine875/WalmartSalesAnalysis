# 🛒 Walmart Sales Analysis

![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

> End-to-end SQL analysis of 1,000+ Walmart sales transactions across 3 branches — uncovering revenue drivers, customer behaviour, and product performance.

---

## 📌 Project Overview

This project explores Walmart sales data from **3 branches** (Mandalay, Yangon, Naypyitaw) to answer key business questions around product performance, sales trends, and customer segmentation. The goal is to identify actionable insights that can help optimize sales strategies.

**Dataset:** [Kaggle — Walmart Sales Forecasting](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting)

---

## 🎯 Objectives

- Identify **top-performing branches and product lines**
- Analyze **sales trends** across time of day, day of week, and month
- Understand **customer behaviour** by type, gender, and payment method
- Calculate **revenue, COGS, VAT, and gross margin** metrics

---

## 📊 Dataset

| Property | Value |
|----------|-------|
| Rows | 1,000 |
| Columns | 17 |
| Branches | 3 (Mandalay, Yangon, Naypyitaw) |
| Source | Kaggle |

**Key columns:** `invoice_id`, `branch`, `city`, `customer_type`, `gender`, `product_line`, `unit_price`, `quantity`, `VAT`, `total`, `date`, `time`, `payment_method`, `cogs`, `gross_income`, `rating`

---

## 🛠️ Approach

### 1. Data Wrangling
- Built MySQL database and created structured table
- Set `NOT NULL` constraints to eliminate missing values at ingestion

### 2. Feature Engineering
Added 3 new columns for deeper time-based analysis:
- `time_of_day` — Morning / Afternoon / Evening
- `day_name` — Day of the week (Mon–Fri)
- `month_name` — Month of the transaction (Jan, Feb, Mar)

### 3. Exploratory Data Analysis (EDA)
Answered 20+ business questions across 3 categories:

**Product Analysis**
- Most selling product line
- Product line with highest revenue and VAT
- Branch performance vs average

**Sales Analysis**
- Revenue by time of day and weekday
- Customer type contributing most revenue
- City with highest tax percentage

**Customer Analysis**
- Gender distribution per branch
- Most common payment method
- Best ratings by time and day

---

## 💰 Revenue & Profit Calculations

```
COGS        = unit_price × quantity
VAT         = 5% × COGS
Total       = VAT + COGS
Gross Income = Total − COGS
Gross Margin = Gross Income / Total Revenue
```

---

## 📁 Files

| File | Description |
|------|-------------|
| `WalmartSalesData.csv` | Raw dataset |
| `SQL_queries.sql` | All SQL queries (wrangling, EDA, feature engineering) |

---

## 🔍 Key Findings

- **Food and Beverages** generated the highest revenue overall
- **Evening hours** consistently recorded the most sales across all branches
- **Female customers** gave slightly higher ratings than male customers
- **Branch C (Naypyitaw)** had the highest average customer rating

---

## 👤 Author

**Mohcine Behate**
- GitHub: [Mohcine875](https://github.com/Mohcine875)
- LinkedIn: [mohcine-behate-3b27a857](https://www.linkedin.com/in/mohcine-behate-3b27a857/)
