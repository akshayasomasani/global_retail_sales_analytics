# 🌍 Global Retail Sales & Customer Analytics Dashboard

## 📌 Project Overview
An end-to-end data analysis project examining global wholesale chocolate and confectionery transactions. The goal of this project was to clean multi-table relational data, engineer financial metrics, and uncover regional and product-level profit drivers to guide executive business decisions.

---

## 🛠️ Tech Stack & Tools Used
* **Python (Pandas, Matplotlib, Seaborn):** Data cleaning, multi-table left joins, column collision management, feature engineering, and data visualization.
* **SQL / Relational Schema Concepts:** Primary/Foreign key relationships (`Sales Person` $\rightarrow$ `SP ID`, `Geo` $\rightarrow$ `GeoID`, `Product` $\rightarrow$ `Product ID`).
* **Microsoft Excel:** Multi-sheet reporting (`retail_final_report.xlsx`), PivotTables, and PivotCharts for executive dashboarding.

---

## 📂 Dataset Structure
The project integrates four relational data sources:
1. **`sales-data.csv`:** Transaction logs (Date, Sales Person, Geo, Product, Amount, Boxes).
2. **`products.csv`:** Product metadata (Product ID, Name, Category, Size, Cost per Box).
3. **`people-tel.csv`:** Sales team directory (Sales Person ID, Name, Team, Location).
4. **`geo.csv`:** Geographic mapping (GeoID, Country, Region).

---

## 🔍 Key Business Insights & Findings
* **Top Profit Category:** **Bars** significantly outperformed other categories, driving over **$16.8M** in total profit.
* **Top Revenue Region:** **APAC (Asia-Pacific)** led global sales revenue with over **$220M**, followed by the Americas ($143M).
* **Financial Feature Engineering:** Created calculated fields for `Total Cost` (`Boxes` * `Cost per Box`) and `Profit` (`Amount` - `Total Cost`) to accurately measure profitability per transaction.

---

## 📊 Visualizations & Reports
* **Python Chart:** Generated automated bar plots via Seaborn displaying profit margins across product categories.
* **Excel Report:** Exported a structured, multi-sheet workbook (`retail_final_report.xlsx`) utilized for interactive PivotTable dashboards.
