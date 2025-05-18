# Amazon-Sales-Analysis

### 📊 Dashboard Preview: 

![image](https://github.com/user-attachments/assets/ea685765-6530-4da0-b7a5-87ac8eb1bbc0)

---

## 🧩 Problem Statement

This dashboard helps Amazon stakeholders analyze sales performance over time and across product categories. It provides visibility into which products are performing best by both revenue and customer satisfaction. The report enables data-driven decisions to optimize product strategies, seasonal planning, and category-level marketing.

---

## ✅ Key Performance Indicators (KPIs)

The dashboard highlights four major KPIs essential for business monitoring:

1. **Year-to-Date (YTD) Sales** – Total revenue generated from the beginning of the year to the current date.
2. **Quarter-to-Date (QTD) Sales** – Revenue generated in the current quarter to date.
3. **YTD Products Sold** – Total number of product units sold year to date.
4. **YTD Reviews** – Total number of customer reviews received during the year.

These KPIs are shown using **card visuals** at the top of the dashboard for quick insights.

---

## 🔍 Dimensions & Visuals Included

### 📅 Time-Based Analysis

- **Sales by Month** – Line chart showing monthly revenue trends across the year.
- **Sales by Week** – Area or bar chart showing weekly sales variations for operational tracking.

### 🗂 Product-Level Analysis

- **Sales by Product Category** – Bar chart summarizing total revenue by category.
- **Top 5 Products by YTD Sales** – Ranked list of best-performing products by total sales.
- **Top 5 Products by Customer Reviews** – Products receiving the most reviews, indicating high customer engagement or popularity.

### 🧮 Filters & Slicers

- **Quarter Selector** – Allows filtering KPIs and visuals based on selected quarter (Q1 to Q4).
- **Product Category Selector** – Enables deep-dives into specific product categories for performance review.

---

## 📈 Data Preparation Steps

1. **Data Loading** – CSV dataset imported into Power BI Desktop.
2. **Power Query Editor** – 
   - Verified column quality, distribution, and null values.
   - Removed or imputed missing values where appropriate.
3. **DAX Measures Created** –
   - `YTD Sales = TOTALYTD(SUM(Sales[Revenue]), Sales[Date])`
   - `QTD Sales = TOTALQTD(SUM(Sales[Revenue]), Sales[Date])`
   - `YTD Products Sold = TOTALYTD(SUM(Sales[Quantity]), Sales[Date])`
   - `YTD Reviews = TOTALYTD(COUNT(Sales[ReviewID]), Sales[Date])`
4. **Time Intelligence** – Added a date dimension for time-based slicing and aggregation.
5. **Visual Design** – Applied theme, title, slicers, and card visuals to enhance readability.

---

## 📌 Insights

- Highest **sales volume** observed in Q4, driven by holiday shopping.
- **Electronics** and **Home & Kitchen** lead in revenue generation.
- A few products account for the **majority of reviews**, indicating focus areas for marketing or quality review.
- Most products with high YTD sales also align with high review counts.

---

## 📤 Deployment

- Final report created using **Power BI Desktop** and exported as a `.pbix` file.
- You can download the report here: [Download Amazon Sales Analysis Report (.pbix)](https://github.com/shubhangi-singh6/Amazon-Sales-Analysis/raw/refs/heads/main/Amazon%20Sales%20Analysis.pbix)

---

> ✅ Use this dashboard to track product performance, optimize inventory, and make strategic decisions for future sales cycles.
