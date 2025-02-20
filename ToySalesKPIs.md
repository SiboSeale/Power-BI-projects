# Toy Store KPI Report

## Project Overview
The **Toy Store KPI Report** is an interactive Power BI dashboard designed to analyze key performance indicators (KPIs) related to toy store sales. The project involves data connection, modeling, measure calculations, and visualization to deliver insights into sales performance, revenue, and profitability.

## Objectives

### Objective 1 - Connecting and Profiling the Data
- Connected to the **sales, products, stores, and calendar** CSV files.
- Reviewed table columns, checked for **blank or null** values, confirmed **data types**, and identified **primary and foreign keys**.
- Added calculated columns in the **calendar table** for `start of month` and `start of week`.

### Objective 2 - Creating a Relational Model
- Loaded tables into the **data model** and established relationships:
  - **Sales table** connected to **Products, Stores, and Calendar** tables.
- Ensured **best practices** for data modeling by implementing a **star schema** with **1:many relationships** between fact and dimension tables.
- Created a **date hierarchy** using `start of month`, `start of week`, and `date` fields.

### Objective 3 - Adding Calculated Measures & Fields
- Created calculated columns in the **Sales table** to reference **cost and price** from the Products table.
- Used these columns to compute **revenue and profit** for each transaction.
- Defined key **measures**:
  - `Total Orders`: Count of orders.
  - `Total Revenue`: Sum of revenue.
  - `Total Profit`: Sum of profit.
- Developed new measures for **total revenue and profit** without relying on calculated columns in the Sales table.

### Objective 4 - Building an Interactive Report
- Added **KPI card visuals** displaying:
  - `Total Orders`, `Total Revenue`, and `Total Profit` for the current month.
  - Monthly trends for each metric.
- Implemented a **slicer** to filter the report by **store location**.
- Created **visualizations**:
  - **Bar chart** showing `Total Orders by Product Category`.
  - **Line chart** illustrating `Total Revenue over time` using the **date hierarchy**.
- Designed an intuitive report layout, adjusted formatting, and ensured a polished final presentation.

## Tools & Technologies Used
- **Power BI** for data modeling and visualization.
- **DAX (Data Analysis Expressions)** for calculated measures and fields.
- **CSV files** as data sources.

## Summary
The **Toy Store KPI Report** delivers valuable insights into toy store performance by leveraging an effective **data model**, **custom measures**, and **interactive visualizations**. The dashboard provides stakeholders with a clear view of key metrics, trends, and store performance.

---

### Next Steps & Enhancements
- Integrate **more advanced DAX calculations** for deeper analytics.
- Implement **dynamic filtering** for enhanced user interactivity.
- Extend the dataset with **customer demographics** to analyze purchasing patterns.
