# PizzaReport_PowerBi

# 1. OverView
I developed an interactive Power BI dashboard to analyze business performance for a pizza seller. The dashboard provides a comprehensive view of key performance indicators, including total revenue, total orders, average order value, and sales trends over time. It also highlights top-selling pizza categories, customer preferences, and peak ordering hours, enabling the seller to identify growth opportunities and optimize decision-making. By transforming raw sales data into meaningful visual insights, this project demonstrates the ability to use data visualization for business intelligence, operational efficiency, and strategic planning.

# 2. Business Problem and Objectives
Business Problem:
The pizza seller had a large volume of sales data but lacked a structured way to monitor and analyze it effectively. Without proper insights, it was difficult to track revenue growth, order trends, best-selling products, and customer behavior. This limited their ability to make data-driven decisions such as identifying peak sales hours, optimizing the menu, managing inventory, and improving marketing strategies.

Objectives:
The primary objective of this project was to design and implement a Power BI dashboard that transforms raw sales data into actionable insights. The key goals were:
- To analyze total revenue and total orders for tracking overall business performance.
- To identify top-selling pizzas and categories that contribute the most to revenue.
- To track sales trends over time and recognize peak order hours or days.
- To calculate average order value and customer buying patterns for better targeting.

To provide a visually interactive dashboard that enables the pizza seller to make informed, data-driven decisions quickly and effectively.

# 3. Dataset Description
Pizza Sales data with 48621 rows and 12 columns data with columns pizza_id,order_id,pizza_name,quantity,order_date,order_time,unit_price,total_price,pizza_category,pizza_ingredients,pizza_name_id

# 4. Methodolgy
The dataset was first cleaned to remove inconsistencies and ensure accuracy. Custom columns were created to enhance time-based analysis:
-Day_Name – Extracted the day of the week from order_date.
-Month_Name – Extracted the month name from order_date.
-Day_Number – Assigned numeric values to weekdays for proper sorting.
-Data types were then adjusted according to their purpose:
-order_date → Date format
-order_time → Time format
-quantity, unit_price, total_price → Numeric format

Additionally, several Key Performance Indicators (KPIs) were created to track overall performance:
-Total Revenue = SUM(pizza_sales[total_price])
-Total Orders = DISTINCTCOUNT(pizza_sales[order_id])
-Total Pizza Sold = SUM(pizza_sales[quantity])
-Average Order Value = [Total_Revenue] / [Total_Orders]
-Average Pizza Per Order = [Total_Pizza_Sold] / [Total_Orders]

These transformations and KPIs provided the foundation for building an insightful and interactive Power BI dashboard.

# 5. Insights and Results
From the analysis of the pizza sales data, the following key insights were derived:
-Order Trends by Day: Orders are highest on weekdays such as Friday, Saturday, and Sunday, indicating peak demand during weekends.
-Monthly Trends: Maximum orders were placed in the months of July and January, showing seasonal demand patterns.
-Top Revenue Contributor: The Thai Chicken Pizza generates the highest revenue among all pizza types.
-Most Ordered Pizza (Quantity): The Classic Deluxe Pizza contributes to the maximum total quantities sold.
-Most Popular Pizza (Orders): The Classic Deluxe Pizza also records the highest number of individual orders.
-Lowest Performer: The Brie Carre pizza contributes the least in terms of revenue, total quantities, and total orders, making it the weakest performer.

# 6. Project Reference
<img width="1335" height="690" alt="image" src="https://github.com/user-attachments/assets/30b8086e-87cd-47e2-8c7f-272d86e73f7c" />
<img width="1565" height="697" alt="image" src="https://github.com/user-attachments/assets/61e1971f-1f32-40b4-955a-fe9eef2c3c95" />

  
