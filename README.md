(Preview.jpeg)

README - Sales Performance Dashboard

Problem Statement

Project Title: Sales Performance Dashboard

Objective:
Build an interactive Power BI dashboard that tracks overall sales performance, profitability, and customer demand across different geographies, categories, and time periods.

Stakeholders:
- Sales Managers (to monitor revenue & profit trends)
- Marketing Teams (to analyze category performance & customer demand)
- Finance (to track profitability & margins)
- Executives (to take decisions on promotions & expansions)

Key Questions:
1. What is the total revenue, profit, and quantity sold over time?
2. Which product categories and sub-categories are performing best/worst?
3. How are sales and profits distributed across states and cities?
4. Which payment modes are most preferred by customers?
5. Who are the top customers driving revenue?

KPIs:
- Total Sales Amount
- Total Profit
- Total Quantity Sold
- Profit Margin % = Profit / Sales Amount
- Orders by Payment Mode
- Sales by Category/Sub-Category
- Regional Sales & Profit

Scope & Constraints:
- Integrates Orders and Details tables using Order ID as key
- Requires data cleaning for missing/null values
- Ensure visualizations are interactive with slicers

Recommended Visualizations:
- KPI cards for Sales, Profit, Quantity, Margin%
- Line/Area chart for trend analysis
- Bar/Treemap for Category/Sub-Category analysis
- Map/Bar for regional performance
- Tables with drill-through for Customers and Orders
- Pie/Donut for Payment Mode

Report Overview

Dashboard Title: Sales Performance Dashboard

Page 1 — Executive Summary
- KPI cards: Total Sales, Total Profit, Quantity Sold, Profit Margin%
- Line chart: Sales Trend over time
- Bar chart: Sales & Profit by Category
- Pie/Donut: Payment Mode distribution

Page 2 — Category & Sub-Category Analysis
- Treemap / Bar chart: Sales & Profit by Category → drill down to Sub-Category
- Profitability heatmap by Category vs Sub-Category
- Table with Top N products by sales/profit

Page 3 — Regional Performance
- Map: Sales & Profit by State
- Bar chart: Top 10 Cities by Sales
- Table: Orders by City with drill-through

Page 4 — Customer Analysis
- Table: Top Customers by Sales & Profit
- KPI: Unique Customers count
- Scatter chart: Sales vs Profit per Customer

Page 5 — Profitability Insights
- Margin trend over time
- High-sales but low-profit categories/products
- Comparison of Profit vs Sales across regions

Filters/Slicers
- Date Range
- Category/Sub-Category
- State/City
- Payment Mode

Key Measures (DAX Examples):
- Total Sales = SUM(Details[Amount])
- Total Profit = SUM(Details[Profit])
- Profit Margin % = DIVIDE([Total Profit],[Total Sales])
- Quantity Sold = SUM(Details[Quantity])
- Orders Count = DISTINCTCOUNT(Orders[Order ID])

End of Document
