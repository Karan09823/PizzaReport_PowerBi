🍕 PizzaReport_PowerBI
1. Overview

I developed an interactive Power BI dashboard to analyze business performance for a pizza seller. The dashboard provides a comprehensive view of key performance indicators, including total revenue, total orders, average order value, and sales trends over time. It also highlights top-selling pizza categories, customer preferences, and peak ordering hours, enabling the seller to identify growth opportunities and optimize decision-making.

By transforming raw sales data into meaningful visual insights, this project demonstrates the ability to use data visualization for business intelligence, operational efficiency, and strategic planning.

2. Business Problem and Objectives
Business Problem

The pizza seller had a large volume of sales data but lacked a structured way to monitor and analyze it effectively. Without proper insights, it was difficult to track revenue growth, order trends, best-selling products, and customer behavior. This limited their ability to make data-driven decisions such as identifying peak sales hours, optimizing the menu, managing inventory, and improving marketing strategies.

Objectives

The primary objective of this project was to design and implement a Power BI dashboard that transforms raw sales data into actionable insights. The key goals were:

To analyze total revenue and total orders for tracking overall business performance.

To identify top-selling pizzas and categories that contribute the most to revenue.

To track sales trends over time and recognize peak order hours or days.

To calculate average order value and customer buying patterns for better targeting.

To provide a visually interactive dashboard that enables the pizza seller to make informed, data-driven decisions quickly and effectively.

3. Dataset Description

The project uses Pizza Sales Data with 48,621 rows and 12 columns.

Dataset Columns:

pizza_id – Unique identifier for each pizza item.

order_id – Unique identifier for each order.

pizza_name – Name of the pizza ordered.

quantity – Number of units ordered.

order_date – Date of order.

order_time – Time of order.

unit_price – Price per unit of pizza.

total_price – Total amount per order (quantity × unit_price).

pizza_category – Category/type of pizza.

pizza_ingredients – List of ingredients used.

pizza_name_id – Encoded identifier for pizza name.

4. Methodology

The dataset was first cleaned to remove inconsistencies and ensure accuracy.

Data Transformations

Custom Columns Created:

Day_Name → Extracted weekday name from order_date.

Month_Name → Extracted month name from order_date.

Day_Number → Assigned numeric values to weekdays for proper sorting.

Data Type Adjustments:

order_date → Date format

order_time → Time format

quantity, unit_price, total_price → Numeric format

KPIs (DAX Measures)

Total Revenue = SUM(pizza_sales[total_price])

Total Orders = DISTINCTCOUNT(pizza_sales[order_id])

Total Pizza Sold = SUM(pizza_sales[quantity])

Average Order Value = [Total_Revenue] / [Total_Orders]

Average Pizza Per Order = [Total_Pizza_Sold] / [Total_Orders]

These transformations and KPIs provided the foundation for building an insightful and interactive dashboard.

5. Insights and Results

Key insights derived from the analysis:

Order Trends by Day: Highest demand on Friday, Saturday, and Sunday, showing weekend peaks.

Monthly Trends: July and January recorded maximum orders, indicating seasonal sales spikes.

Top Revenue Contributor: Thai Chicken Pizza generated the highest revenue.

Most Ordered Pizza (Quantity): Classic Deluxe Pizza contributed to the highest total quantity sold.

Most Popular Pizza (Orders): Classic Deluxe Pizza also recorded the highest number of orders.

Lowest Performer: Brie Carre Pizza had the lowest revenue, quantity sold, and total orders.

6. Project Reference

📊 Dashboard Screenshots:

<img width="1335" height="690" alt="Pizza Dashboard 1" src="https://github.com/user-attachments/assets/30b8086e-87cd-47e2-8c7f-272d86e73f7c" /> <img width="1565" height="697" alt="Pizza Dashboard 2" src="https://github.com/user-attachments/assets/61e1971f-1f32-40b4-955a-fe9eef2c3c95" />
7. Conclusion & Recommendations

The Power BI dashboard provided clear insights into sales performance, customer preferences, and product contributions.

Recommendations for the Pizza Seller:

Focus on promoting top-selling pizzas (Thai Chicken Pizza, Classic Deluxe Pizza) to boost revenue further.

Reconsider or market-test low-performing items like Brie Carre.

Plan marketing campaigns around weekends and peak months (July & January) to maximize sales.

Use insights on average order value and pizzas per order to design attractive combo offers.

This analysis empowers the pizza seller to make data-driven decisions, optimize the menu, and improve business performance.
