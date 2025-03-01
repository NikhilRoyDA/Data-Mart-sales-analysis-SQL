# Data Mart Sales Performance Analysis 🚀  

## 📌 Project Overview  
This project analyzes **Data Mart’s sales performance** to measure the impact of **sustainable packaging changes** introduced in June 2020. Using **SQL**, I transformed raw sales data into actionable insights, focusing on sales trends across **regions, platforms, and customer demographics**.  

## 📊 Key Highlights  
- 🛠 **Tech Used:** SQL (CTEs, Window Functions, Aggregations)  
- 🏪 **Data:** 340M+ transactions from 3 years  
- 📈 **Analysis:** Retail vs. Shopify performance, customer demographics, revenue trends  

## 🔍 Insights Discovered  
- **Retail outperformed Shopify** in monthly sales.  
- **Retirees and Families** were the biggest spenders in Retail.  
- **Seasonal trends** affected sales volume.  

## 📁 Repository Structure  
-- Identifying missing weeks in the dataset
WITH week_series AS (
    SELECT generate_series(
        (SELECT MIN(week_date) FROM clean_weekly_sales),
        (SELECT MAX(week_date) FROM clean_weekly_sales),
        INTERVAL '1 week'
    ) AS week_date
)
SELECT week_date
FROM week_series
LEFT JOIN clean_weekly_sales USING (week_date)
WHERE clean_weekly_sales.week_date IS NULL;


