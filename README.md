# Power BI Dashboard / Project: Superstore Sales Data Analytics #

![Home Page](/Images/Our%20Superstore.jpg)

## Introduction & Project Overview ##

This dashboard was created for a **Sales / Business Development Manager of a global SuperStore**. It focuses on analyzing sales data from the superstore to **uncover actionable insights about sales performance, product categories, and consumer behavior**. The goal is to demonstrate how raw sales data can be transformed into meaningful information to support data-driven strategic decisions in sales and business development.

By using Power BI, I designed several interactive dashboards that provide:

1. 📈 Sales Insights – overall Sales growth and seasonal patterns
2. 🛍️ Product Insights – best and worst-performing categories , sub-categories, and products
3. 👥 Customer Analysis – consumer segments contributing most to sales
4. 🌍 Regional Performance – sales distribution across different regions or markets


## 🛠️ Skills Demonstrated ##

This project demonstrates the end-to-end Power BI workflow, covering data preparation, modeling, analysis, and dashboarding.

🔄 Data Preparation / ETL Process (Power Query)

- 📥 Extracted raw sales data from the web and created Fact (Sales) and Dimension (Customer, Product) tables.

- 🧹 Cleaned and transformed data: removed unnecessary columns, handled blanks/errors, ensured correct data types.

- 🔑 Removed duplicates from dimension tables to maintain integrity.

🗂️ Data Modeling

- 📅 Built separate Date Tables (Order & Shipping) for accurate time-series analysis (Year-over-Year, Month-over-Month).

- ⭐ Designed a Star Schema with fact (Sales Table) and dimension tables (Customer Table, Product Table, Order Date Table, Shipping Date Table).

- 🔗 Established 1-to-many relationships for consistent insights.

📊 Data Analysis (DAX)

- ➕ Created calculated columns and measures: Total Sales / Revenue, Total sales for a specific year / Region / category, Total Profit, Profit Margin, Total Orders, Distinct Categories.

- 🧮 Applied functions like CALCULATE, SUMX, DIVIDE, DISTINCTCOUNT, COUNTA.

- ⏳ Enabled time intelligence with CALENDAR, YEAR, MONTH, DAY.

📈 Data Visualization

- 📉 Line Charts → To show Sales & Profit trends (Year-over-Year, Month-over-Month, Quater-over-Quater).

- 🗂️ Cards → To demonstrate Key KPIs (Total No. of Orders, Total Sales, Total Profit, and Profit Margin).

- 📊 Bar/Column/Cluster Column/Stacked Bar Charts → To compare Total Sales / Overall Performance by category, Products, consumer segment, and region.

- 🥧 Pie Chart → To exhibit Shipping mode distribution.

🎛️ Interactive Dashboard

- 🎛️ Added slicers, drill-downs, tooltips, and navigation buttons for interactivity.

- 🎨 Delivered a business-friendly, interactive dashboard that supports strategic decision-making.


## Data Structure / Model Overview ##

![Data Model](/Images/Data%20Model.jpg)
This is the model view of our dashboard. As you can see in the model, we have total 6 tables in the model: Customer table, Product table, Sales table, Order date table, Ship date table, and All Measure Table. However, In the original dataset, we had just one flat "Superstore sales Table". We have created separate "Customer Table" and "Product Table" to normalize the data. In addition, we have also created separate "Ship Date" and "Order Date" Table to avoid confusion or mismatch during Time Series Analysis. Then, we have built a Star Schema where all dimension tables relate to Fact Table (Sales Table) via 1-to-Many relationship, filter directing from dimension to fact table. "_All Measure" is a separate table which we have created to store our all measures in one place.   


## Dashboard Overview: Executive Summary / Key Insights ##

### Sales Insights ###

![Overall Sales Insights](/Images/Sales%20Insights_Overall.jpg)

This is the overall sales insights dashboard. It highlights key KPIs like Total orders, Total Sales, Total Profit, and Profit Margin. This also compares year-over-year Total Sales and Profit Growth. The Dashboard shows following insights: 

1. The Revenue has increased over the years. After slightly decreasing between 2014 and 2015, the revenue has significantly improved between 2015 and 2017, with highest jump between 2015 and 2016.

2. The Profit has consistently increased over the years. Between 2014 & 2015, the profit has increased by 24%, followed by 33% and 14% respectively in the following years. Even though Profit has consistently increased over the years, overall Profit Margin has been quite low over the years, stand at 2.89%.

3. Across all years, it has been shown that Qtr-4 is the highest selling period, followed by Qtr-3, Qtr-2, and Qtr-1. 

### Product Insights ###

![Overall Product Insights](/Images/Product%20Insights_Overall.jpg)

This is the overall product insights dashboard. It compares product categories and sub-categories as well as shows best and worst performing products in terms of total sales or revenue for complete data (means without applying any filter). Users can drill down by year or region for more specific insights. For Example, See the next image.


![Product Insights Drill-down for a specific year (2014) & for a specific region (south)](/Images/Product%20Insights%20Drill-Down%20for%20a%20specific%20year%20(2014)%20with%20a%20specific%20Region%20(South).jpg)

This is the product insights drill-down for the year 2014 and for the region south. Best- and worst-performing products differ significantly compared to the overall dataset, highlighting the importance of regional analysis.

### Consumer Insights ###

![Overall Consumer Insights](/Images/Consumer%20Insights_Overall.jpg)

This is the overall consumer insights dashboard. It demonstrates which consumer segment, region, and states contributing most to our revenue (cover complete data, means without applying any filter). It also reveals product preferences by segment and geography. This page can also be drill-down by a specific year to see year specific details. For instance, see the next image.


![Consumer Insights Drill-down for a specific year 2014](/Images/Consumer%20Insights%20Drill-Down%20for%20a%20specific%20year%20(2014).jpg)

This is the consumer insights drill-down for the year 2014. Results vary significantly compared to the overall dataset, allowing deeper exploration of consumer behavior.


## Conclusion

The Superstore Sales Data Analytics project demonstrates how raw sales data can be transformed into actionable business insights using Power BI. Through structured data preparation, modeling, DAX calculations, and interactive visualization, the dashboard provides a 360° view of sales, products, and consumer behavior.

**Key Insights Delivered:**

- 📈 Identified overall and year-specific sales & profit growth trends.

- 🛍️ Highlighted best- and worst-performing products, product categories, and sub-categories across regions and time-frames.

- 👥 Analyzed customer segments and geographic markets contributing most to revenue.

- 🎛️ Delivered an interactive, user-friendly dashboard that supports data-driven decision-making for business development and sales strategy.

**Key Takeaways from this project**

- I understood the importance of proper data modeling (Star Schema) to ensure accurate and efficient analysis.

- I practiced writing DAX measures for KPIs such as profit margin, sales growth, and customer segmentation, which deepened my understanding of DAX functions.

- I learned how much value interactive features (slicers, drill-downs, tooltips, navigation) bring to a dashboard, making it easier for users to explore insights on their own.

- Most importantly, I realized that data visualization is not just about charts—it’s about telling a story that supports business planning.

Overall, this project improved both my technical Power BI skills and my ability to think from a business perspective. It reflects my ability to design, build, and deliver BI solutions that not only visualize data but also provide meaningful insights for strategic planning.
