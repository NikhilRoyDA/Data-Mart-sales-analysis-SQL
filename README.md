# Data Mart Sales Performance Analysis 🚀  

## 📌 Project Overview  
This project analyzes **Data Mart’s sales performance** to measure the impact of **sustainable packaging changes** introduced in June 2020. Using **SQL**, I transformed raw sales data into actionable insights, focusing on sales trends across **regions, platforms, and customer demographics**.  

## 🛠 Tech Stack Used  
- **SQL:** CTEs, Window Functions, Aggregations, Joins  
- **Database:** PostgreSQL / MySQL  
- **BI Tools (Optional):** Tableau / Power BI (For Visualization)  
- **GitHub:** Version control & project documentation  

---

## 📂 Dataset Information - [Schema](https://github.com/NikhilRoyDA/Data-Mart-sales-analysis-SQL/tree/main/Schema)
- **Total Transactions:** ~340M  
- **Time Frame:** 3 years (Before & After June 2020)  
- **Key Data Points:**  
  - `week_date`: Sales date in weekly format  
  - `region`: Sales distribution across different geographical areas  
  - `platform`: Comparison between **Retail & Shopify**  
  - `customer_type`: **Retirees, Families, Young Adults, etc.**  
  - `sales_amount`: Total revenue generated  

---

## 🔍 Key Analysis & Insights - <a heref"https://github.com/NikhilRoyDA/Data-Mart-sales-analysis-SQL/blob/main/Assignment%20%26%20Insights/Insights%20%20-%20DATA%20MART%20Analysis.pdf"<Insights>a

### 📌 **1. Data Cleaning & Transformation**  
- Standardized the **date format** to weekly (`week_date`).  
- Created a structured **clean_weekly_sales** table.  
- Segmented customers into **age groups & demographics**.  
- Filled missing values and handled anomalies.  
- Derived **new columns**: `week_number`, `month_number`, `age_band`, `demographic`.  

---

### 📌 **2. Exploratory Data Analysis (EDA)**  
- Identified **missing weeks** in the dataset using sequence generation.  
- Analyzed **total yearly transactions** (~340M).  
- Compared **Retail vs. Shopify sales contribution** per month.  
- **Discovered key trends** in sales across regions & customer segments.  

📌 **Insights Discovered:**  
✔️ **Retail consistently outperformed Shopify** in monthly sales.  
✔️ **Retirees & Families** contributed the most to Retail sales.  
✔️ **Sales dips** during off-seasons & peaks during holidays.  

---

### 📌 **3. Advanced SQL Techniques Used**  
✔️ **CTEs (Common Table Expressions)** – Used for structured queries.  
✔️ **Window Functions** – For running totals & trend analysis.  
✔️ **CASE Statements** – To create conditional categories for segmentation.  



