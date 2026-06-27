# bushraanjum_2511048_part4_tableau_dashboard
## Project Overview

This project focuses on designing an Executive Tableau Dashboard for retail business leadership. The objective is to transform transactional sales data into actionable business insights that support strategic decision-making.

The dashboard was built to help leadership monitor sales performance, profitability, customer segments, regional trends, shipping efficiency, discount effectiveness, and product return patterns. Rather than presenting isolated charts, the dashboard tells a connected business story that highlights opportunities, risks, and areas requiring management attention.

---

# Business Problem

Retail leadership teams need a centralized view of business performance to make informed decisions regarding growth, profitability, inventory planning, customer management, and operational efficiency.

Key business questions addressed include:

* How are sales changing over time?
* Which regions are driving business performance?
* Which product categories are most profitable?
* How do customer segments contribute to revenue?
* What impact do discounts have on profitability?
* Which shipping methods create operational risks?
* Where are product returns concentrated?
* What business opportunities and risks should leadership prioritize?

The Tableau dashboard provides a visual solution to answer these questions.

---

# Dataset Description

**Dataset File:**

dashboard_sales_data.xlsx

The dataset contains retail transaction information including:

* Order Date
* Region
* Customer Segment
* Product Category
* Sub-Category
* Sales
* Profit
* Discount
* Quantity
* Shipping Mode
* Delivery Days
* Customer Rating
* Return Status

The dataset combines financial, operational, customer, and logistics information required for executive-level analysis.

---

# Tableau Workbook

**Workbook File:**

tableau/executive_dashboard.twbx

The Tableau workbook contains multiple worksheets and one integrated executive dashboard designed for leadership reporting.

The workbook includes:

* KPI Sheets
* Analytical Views
* Interactive Filters
* Dashboard Actions
* Executive Dashboard Layout

---

# Calculated Fields Created

Several calculated fields were created to improve business analysis.

### 1. Profit Margin

Formula:

Profit / Sales

Purpose:

Measures profitability efficiency and identifies categories or regions generating stronger returns.

---

### 2. Cost

Formula:

Sales - Profit

Purpose:

Estimates product and operational cost contribution.

---

### 3. Average Order Value (AOV)

Formula:

Sales / COUNT(Order ID)

Purpose:

Measures average revenue generated per order.

---

### 4. Return Rate

Formula:

SUM(Return Flag) / COUNT(Order ID)

Purpose:

Measures the percentage of returned orders and highlights quality or fulfillment issues.

---

### 5. Shipping Delay Bucket

Formula Logic:

* 0–2 Days → Fast Delivery
* 3–5 Days → Standard Delivery
* 6+ Days → Delayed Delivery

Purpose:

Categorizes delivery performance into meaningful business groups.

---

# Dashboard Components

## KPI Cards

The dashboard contains executive KPI cards for quick performance monitoring:

* Total Sales
* Total Profit
* Profit Margin
* Return Rate
* Average Order Value

These KPIs provide leadership with an immediate understanding of overall business health.

---

## Analytical Views

### Sales Trend View

Displays sales performance over time.

Business Purpose:

Monitor growth patterns and identify seasonality.

Visualization Used:

Line Chart

---

### Regional Performance View

Displays sales and profitability by region.

Business Purpose:

Identify geographic strengths and weaknesses.

Visualization Used:

Bar Chart

---

### Category Profitability View

Displays profit contribution across categories and sub-categories.

Business Purpose:

Understand which products create the most business value.

Visualization Used:

Horizontal Bar Chart

---

### Customer Segment View

Compares performance across customer segments.

Business Purpose:

Evaluate customer value and segment behavior.

Visualization Used:

Bar Chart

---

### Shipping Performance View

Analyzes shipping mode performance and delivery delays.

Business Purpose:

Identify logistics risks and operational inefficiencies.

Visualization Used:

Bar Chart

---

### Discount vs Profit View

Examines the relationship between discount levels and profitability.

Business Purpose:

Evaluate pricing strategy effectiveness.

Visualization Used:

Scatter Plot

---

### Return Analysis View

Investigates return patterns by category, region, and customer segment.

Business Purpose:

Identify quality or fulfillment issues impacting profitability.

Visualization Used:

Bar Chart

---

# Filters and Dashboard Interactions

Interactive filters were implemented to improve dashboard usability.

### Filters Used

* Region
* Category
* Customer Segment
* Ship Mode

### Dashboard Interaction

Users can filter the dashboard dynamically and immediately observe changes across all visualizations.

Example:

Selecting:

* Region = West
* Category = Technology

updates all dashboard views simultaneously, allowing leadership to perform focused analysis.

---

# Key Business Insights

### Insight 1

Sales performance remains relatively stable across the observed period, indicating consistent customer demand.

### Insight 2

Regional performance varies significantly, suggesting opportunities for targeted investment and optimization.

### Insight 3

Some product categories generate strong sales but relatively lower profits, highlighting margin concerns.

### Insight 4

Customer segments contribute differently to revenue and profitability.

### Insight 5

Higher discounts are frequently associated with lower profit margins.

### Insight 6

Certain shipping methods show longer delivery times and may affect customer satisfaction.

### Insight 7

Returns are concentrated in specific product categories, creating profitability risk.

### Insight 8

High-performing categories and regions present opportunities for growth and resource allocation.

---

# Dashboard Story Summary

The dashboard tells a business story centered around revenue generation, profitability, operational performance, and customer behavior.

The analysis shows that while overall sales remain strong, profitability is influenced by discounting practices, shipping performance, and product return rates.

Leadership can use the dashboard to:

* Monitor overall business health
* Identify profitable growth opportunities
* Detect operational risks
* Improve customer experience
* Optimize pricing and inventory decisions

---

# Business Recommendations

Based on dashboard findings:

1. Reduce excessive discounting in margin-sensitive categories.
2. Expand investment in high-performing regions.
3. Improve delivery performance for delayed shipping modes.
4. Investigate root causes behind product returns.
5. Prioritize profitable product categories and customer segments.
6. Continue monitoring KPI trends through executive reporting.

---

# Assumptions and Limitations

### Assumptions

* Source data is accurate and complete.
* Return flags correctly represent returned orders.
* Delivery days accurately reflect shipping performance.

### Limitations

* Dashboard provides descriptive analysis rather than causal analysis.
* External market conditions are not included.
* Customer lifetime value is not analyzed.
* Competitor performance data is unavailable.

---

# Screenshots Included

The repository includes the following dashboard evidence:

* full_dashboard.png
* sales_trend_view.png
* regional_performance_view.png
* category_profitability_view.png
* filter_interaction_view.png

These screenshots demonstrate dashboard functionality, chart design, and filter interaction.

---

# Conclusion

This Tableau Executive Dashboard successfully converts raw retail transaction data into a business-focused decision-support tool. Through KPI monitoring, interactive filtering, and visual storytelling, the dashboard enables leadership to identify trends, improve profitability, reduce risk, and make data-driven business decisions.
