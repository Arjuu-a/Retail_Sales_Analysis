# 🛒 Retail Sales SQL Analysis Project

![SQL](https://img.shields.io/badge/SQL-MySQL%208.0-blue)
![Power BI](https://img.shields.io/badge/PowerBI-Visualization-yellow)
![Status](https://img.shields.io/badge/Project-Complete-success)
![Dataset](https://img.shields.io/badge/Records-10,000-informational)

---

## 📌 Project Overview

This project performs an end-to-end business analysis on a **10,000-record retail sales dataset** using SQL.

The objective is to derive actionable business insights related to:

- 📈 Sales performance
- 💰 Profitability & margins
- 🛍 Product performance
- 🌍 Regional contribution
- 👥 Customer behavior
- ⚙ Operational efficiency

The analysis simulates real-world retail business reporting scenarios.

---

## 🎯 Business Objectives

✔ Analyze sales trends and month-over-month growth  
✔ Identify top and bottom performing products  
✔ Evaluate profitability by category and product  
✔ Segment customers and identify repeat buyers  
✔ Perform Pareto (80/20) analysis  
✔ Detect low-margin outliers  
✔ Support data-driven decision-making  

---

## 🛠 Tools & Technologies

- **SQL (MySQL 8.0)** – Data analysis & window functions  
- **Power BI** – Dashboard visualization  
- **GitHub** – Version control & project documentation  

---

## 🗂 Database Schema

```sql
CREATE TABLE retail_sales (
    order_id INT PRIMARY KEY,
    order_date DATE,
    customer_id INT,
    customer_segment VARCHAR(50),
    region VARCHAR(50),
    product_id INT,
    product_name VARCHAR(100),
    category VARCHAR(50),
    sales DECIMAL(10,2),
    quantity INT,
    profit DECIMAL(10,2),
    order_priority VARCHAR(20)
);
```

---

## 📊 Key SQL Analyses Performed

### 1️⃣ Overall Sales & Profit Performance
- Total Orders
- Total Sales
- Total Profit

### 2️⃣ Monthly Sales Trend
- Aggregated monthly revenue
- Time-based trend analysis

### 3️⃣ Month-over-Month (MoM) Growth
- Used `LAG()` window function
- Percentage growth calculation

### 4️⃣ Profitability & Margin Analysis
- Category-wise sales
- Profit margin %

### 5️⃣ Top 10 Products by Sales
- Revenue leaders

### 6️⃣ Bottom 10 Products by Profit
- Underperforming products

### 7️⃣ Region-wise Performance
- Sales and profit by region

### 8️⃣ Customer Segment Contribution
- Segment-based order and sales analysis

### 9️⃣ Repeat vs New Customers
- Identified returning customers
- Measured customer retention

### 🔟 Order Priority Analysis
- Operational insights by priority level

### 1️⃣1️⃣ Inventory & Demand Analysis
- Total quantity sold by product

### 1️⃣2️⃣ Average Order Value (AOV)
- Revenue per order

### 1️⃣3️⃣ Pareto (80/20) Analysis 🔥
- Cumulative revenue contribution
- Identified top revenue-driving products

### 1️⃣4️⃣ Rolling 3-Month Sales Average
- Time-series smoothing
- Window functions with frame clauses

### 1️⃣5️⃣ Outlier Detection
- Identified low-margin products (<5%)

---

## 📈 Advanced SQL Concepts Used

- Common Table Expressions (CTEs)
- Window Functions (`LAG()`, `SUM() OVER()`, `AVG() OVER()`)
- Rolling averages
- Cumulative percentage calculations
- Aggregate functions
- Subqueries
- Grouping & filtering
- Profit margin computations

---

## 📊 Business Insights Derived

- A small percentage of products drive majority revenue (Pareto principle).
- Certain categories generate high sales but low margins.
- Repeat customers significantly impact total revenue.
- Regional sales contribution varies significantly.
- Some products consistently show low profit margins and require pricing review.

---

## 🚀 Business Impact

This analysis supports:

- Pricing optimization
- Inventory planning
- Customer retention strategy
- Regional sales focus
- Product rationalization
- Operational prioritization

---

## 📈 Potential Dashboard Integration

The SQL outputs can be directly connected to **Power BI** to build:

- Sales Trend Dashboard
- Profitability Dashboard
- Customer Insights Dashboard
- Product Performance Dashboard

---

## 🧠 What This Project Demonstrates

✔ Strong SQL fundamentals  
✔ Window function expertise  
✔ Business KPI modeling  
✔ Analytical thinking  
✔ Real-world reporting capability  

---

## 📂 Suggested Repository Structure

```
Retail-Sales-SQL-Analysis/
│
├── sql/
│   ├── create_table.sql
│   ├── analysis_queries.sql
│
├── powerbi/
│   └── retail_dashboard.pbix
│
├── data/
│   └── retail_sales_sample.csv
│
└── README.md
```

---

## 👤 Author

**Jaya Nagarjun**  
Aspiring Data Analyst | SQL | Power BI | Business Intelligence  

---

⭐ If you found this project useful, feel free to star the repository!
