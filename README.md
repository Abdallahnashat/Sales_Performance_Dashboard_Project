# 📊 Sales Performance & Target Achievement Analysis — Power BI

An end-to-end Power BI dashboard built to help sales leadership track **actual vs. target sales performance**, understand **why targets are missed**, and **rank sales team performance** across products, channels, and time.

---

# 🎯 Business Problem

Sales data was scattered across actual sales, monthly targets, product, and sales-team records. Leadership had no single view to answer:

- Are we achieving our sales targets overall and across different time periods?
- Which products, channels, and salespeople are driving or missing performance?
- What factors contribute most to the gap between Actual Sales and Target Sales?
- How has sales performance changed over time?

This dashboard consolidates the data into a single interactive report, enabling decision-makers to monitor performance, identify root causes, and take data-driven actions.

---

# 📊 Dashboard Preview

## Overview

![Overview](images/overview.png)

## Filters Panel

![Filters](images/filters.png)

## Ranking

![Ranking](images/ranking.png)

## Custom Tooltips

Achievement Gauge tooltip, shown on hover — turns red when performance dips below target:

![Achievement Below Target](images/achievement_below_target.png)
![Tooltip](images/tooltip.png)

---

# 🗂️ Data Model

The report follows a **Star Schema** consisting of two fact tables connected to shared dimensions for consistent filtering and efficient analysis.

![Data Model](images/data_model_star_schema.png)

| Table | Type |
|--------|------|
| `FactSales` | Fact |
| `TargetSales` | Fact |
| `DimDate` | Dimension |
| `DimProduct` | Dimension |
| `DimSalesPerson` | Dimension |

Shared dimensions (`Date`, `Product`, and `Salesperson`) filter both fact tables, ensuring consistent KPI calculations and time-based analysis across the report.

---

# 📄 Report Pages

## 1. Overview

The landing page provides a high-level summary of sales performance through:

- KPI cards (Actual Sales, Target Sales, Achievement %, Orders, Quantity)
- Sales trend over time
- Channel and product category breakdowns
- Interactive matrix
- Dynamic slicers for Year, Channel, Product, and Salesperson

---

## 2. Variance Analysis

Uses a **Decomposition Tree** to investigate the gap between Actual and Target Sales.

Users can drill down by:

- Product
- Salesperson
- Time Period

to quickly identify the primary drivers behind sales performance.

---

## 3. Ranking

Ranks salespeople based on their performance using:

- Achievement %
- Total Sales
- Sales Rank
- Profile photos for better presentation

---

## 4. Custom Tooltips

Dedicated tooltip pages provide additional context without cluttering the report, including:

- Achievement Gauge
- Product Group Details

---

# 📈 Key Insights

The dashboard enables business users to:

- Monitor actual sales against targets in real time.
- Identify products and salespeople contributing most to performance gaps.
- Track sales trends across months, quarters, and years.
- Compare sales performance across channels and product categories.
- Rank salespeople based on achievement percentage and total sales.
- Perform root-cause analysis through interactive drill-downs.

---

# 🛠️ Skills Demonstrated

- Power BI
- Data Modeling
- Star Schema Design
- DAX
- Time Intelligence
- Variance Analysis
- KPI Design
- Interactive Dashboard Development
- Decomposition Tree
- Custom Tooltips
- Conditional Formatting
- Bookmarks & Navigation
- Business Intelligence Reporting