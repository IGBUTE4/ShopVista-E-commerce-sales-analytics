# ShopVista-E-commerce-sales-analytics

## 📊 Project Overview

This project analyzes sales data from an online retail business to uncover trends in revenue, orders, products, regions, and customer behavior.

The project follows an end-to-end data analytics workflow, beginning with data cleaning and transformation using **SQL Server**, followed by data modeling, DAX calculations, visualization, customer analysis, and business insights in **Power BI**.

The objective was not only to build a dashboard, but to transform raw transactional data into actionable insights that can support business decision-making.

<img width="1281" height="2286" alt="Screenshot_30-9-2026_31622_" src="https://github.com/user-attachments/assets/165ff97c-9aee-4a02-8543-5b16de9af7a8" />
<img width="578" height="323" alt="Screenshot 2026-09-30 031258" src="https://github.com/user-attachments/assets/e5ec3812-e392-44ab-b37e-6490c9666de2" />


---

## 🎯 Business Objectives

The analysis was designed to answer key business questions such as:

* How is overall sales performance changing over time?
* How does current-year revenue compare with the previous year?
* Which regions generate the most revenue?
* Which products and categories contribute the most to revenue?
* How concentrated is revenue among the top-performing products?
* How frequently are customers purchasing?
* Which customers are highly valuable to the business?
* What does customer recency, frequency, and monetary behavior reveal?
* Which areas of the business require attention or further investigation?

---

## 🛠️ Tools & Technologies

* **SQL Server** — Data cleaning, transformation, validation, and analysis
* **Power BI** — Data modeling, DAX, visualization, and dashboard development
* **DAX** — Measures, time intelligence, customer analysis, and segmentation
* **Excel** — Initial data inspection and supporting analysis

---

## 🗂️ Dataset Structure

The project uses relational sales data consisting of:

### Sales

* SaleID
* CustomerID
* ProductID
* SaleDate
* Quantity

### Products

* ProductID
* ProductName
* Category
* Price

### Customers

* CustomerID
* CustomerName
* CustomerType
* Region

The sales data was cleaned and transformed before being used for analytical reporting.

---

# 🧹 Data Cleaning & Preparation

SQL was used to prepare the raw data for analysis.

Key cleaning activities included:

* Identifying and removing duplicate records
* Handling missing and invalid quantities
* Removing records with non-positive quantities where appropriate
* Standardizing inconsistent text values
* Correcting inconsistent regional naming
* Converting columns to appropriate data types
* Validating relationships between the sales, product, and customer tables
* Creating cleaned datasets for downstream analysis

The final cleaned tables were used as the foundation for the Power BI data model.

---

# 🔎 SQL Analysis

The SQL analysis focused on extracting business metrics and identifying patterns within the data.

### Key analyses included:

* Total revenue
* Total orders
* Total units sold
* Average Order Value (AOV)
* Revenue trends over time
* Monthly and yearly performance
* Year-over-year revenue comparison
* Revenue by region
* Revenue by product category
* Top-performing products
* Revenue contribution
* Customer revenue
* Customer purchase frequency
* Customer activity
* Customer segmentation

SQL queries used techniques including:

* `CTEs`
* `CASE`
* `GROUP BY`
* `JOIN`
* `UNION`
* Window functions
* `ROW_NUMBER()`
* `LAG()`
* Aggregations
* Date functions
* Conditional calculations

The complete SQL analysis is available in the repository.

---

# 📊 Power BI Dashboard

The cleaned data was imported into Power BI and transformed into an interactive analytical report.

The dashboard was designed around four major analytical areas.

## Page 1 — Executive Overview

Provides a high-level view of business performance, including:

* Total Revenue
* Revenue vs Previous Year
* Orders
* Average Order Value
* Units Sold
* Unique Customers
* Revenue trends
* Regional performance
* Category performance
* Top-performing products

The page is designed to provide management with a quick overview of the business.

---

## Page 2 — Product & Regional Performance

Focuses on understanding where revenue is being generated.

Analysis includes:

* Product performance
* Top 5 products
* Top-product revenue contribution
* Category performance
* Regional revenue
* Regional contribution
* Customer and order performance by region
* Average Order Value by region
* Revenue per customer
* Product performance by units, price, and revenue

This page helps identify the products, categories, and regions contributing most significantly to overall performance.

---

## Page 3 — Customer Analysis

Examines customer behavior and engagement.

Key areas include:

* Unique customers
* Customer purchasing activity
* Customer recency
* Purchase-frequency segmentation
* Customer revenue
* RFM analysis
* Customer segments

The analysis provides a deeper understanding of customer value and purchasing behavior.

---

## Page 4 — Insights & Recommendations

The final page translates the analytical findings into business-focused insights.

It summarizes:

* Major performance trends
* Key product and regional findings
* Customer behavior patterns
* Areas requiring attention
* Potential opportunities
* Recommended actions based on the analysis

The purpose of this page is to bridge the gap between **data visualization and business decision-making**.

---

# 📈 Key Analytical Techniques

### Year-over-Year Analysis

Current-period performance was compared with the equivalent previous-year period using DAX time-intelligence calculations.

### Customer Analysis

Customers were evaluated based on their purchasing activity, revenue contribution, purchase frequency, and recency.

### RFM Analysis

Customers were analyzed using:

* **Recency** — How recently the customer purchased
* **Frequency** — How often the customer purchased
* **Monetary Value** — How much revenue the customer generated

These dimensions were combined to identify meaningful customer segments.

### Revenue Contribution

Revenue contribution calculations were used to understand how much of total revenue was generated by:

* Top products
* Regions
* Categories

---

