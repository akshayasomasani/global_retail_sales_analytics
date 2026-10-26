# Global Retail Sales & Customer Analytics

End-to-end data analysis pipeline integrating relational CSV tables (Sales, Products, People, Geo) using Python & Pandas, with multi-table LEFT JOINs to generate executive insights and Excel dashboard reports.

## Project Structure & Workflow
- **Data Preprocessing & Merging:** Cleaned and combined four relational datasets (`sales.csv`, `products.csv`, `people.csv`, `geo.csv`) using Python (Pandas) multi-table `LEFT JOIN` operations.
- **SQL / Relational Schema Concepts:** Designed primary/foreign key relationships (`sales.product_id` -> `products.product_id`, etc.).
- **Microsoft Excel:** Multi-sheet reporting ([retail_final_report.xlsx](retail_final_report.xlsx)), PivotTables, and PivotCharts for executive dashboarding.

## Dataset Structure
The project integrates four relational data sources:
1. **sales-data.csv** : Transaction logs (Date, Sales Person, Geo, Product, Amount, Boxes).
2. **products.csv** : Product metadata (Product ID, Name, Category, Size, Cost per Box).
3. **people-tel.csv** : Sales team directory (Sales Person ID, Name, Team, Location).
4. **geo.csv** : Geographic mapping (GeoID, Country, Region).

## Key Business Insights & Findings
- **Top Profit Category:** Bars significantly outperformed other categories, driving over $16.8M in total profit.
- **Top Revenue Region:** APAC (Asia-Pacific) led global sales revenue with over **$22M+**, followed by the Americas ($143M).
- **Financial Feature Engineering:** Created calculated fields for `Total Cost` (`Boxes` * `Cost per Box`) and `Profit` (`Amount` - `Total Cost`) to accurately measure profitability per transaction.

## Visualizations & Reports
- **Python Chart:** Generated automated bar plots via Seaborn displaying profit margins across product categories.
- **Excel Report:** Exported a structured, multi-sheet workbook ([retail_final_report.xlsx](retail_final_report.xlsx)) utilized for interactive PivotTable dashboards.
