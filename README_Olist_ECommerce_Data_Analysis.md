# Olist Brazilian E-Commerce Data Analysis

![Project](https://img.shields.io/badge/Project-Olist%20E--Commerce%20Analysis-0A66C2)
![Excel](https://img.shields.io/badge/Tool-Excel-217346)
![Power%20Query](https://img.shields.io/badge/Tool-Power%20Query-742774)
![Power%20Pivot](https://img.shields.io/badge/Tool-Power%20Pivot-5B9BD5)
![DAX](https://img.shields.io/badge/Language-DAX-F2C811)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📌 Project Overview

This project analyzes the **Brazilian Olist E-Commerce dataset** to understand sales performance, customer behavior, payment patterns, product and seller performance, delivery performance, and customer satisfaction.

The project was developed as a practical end-to-end **Data Analysis and Business Intelligence project using Microsoft Excel**, including data cleaning, transformation, data modeling, DAX measures, PivotTables, and interactive dashboards.

---

## 🎯 Business Objectives

The analysis aims to answer key business questions such as:

- How did sales change over time?
- Which product categories generated the highest sales?
- Which products and sellers contributed most to sales?
- Which Brazilian states generated the highest sales?
- What payment methods were most frequently used?
- How were installment payments distributed?
- How long did orders take to be delivered?
- What percentage of orders were delivered on time?
- How does delivery performance relate to customer review scores?
- Which areas require business or logistics attention?

---

## 🗂️ Dataset

The project uses the **Olist Brazilian E-Commerce Public Dataset**, which contains approximately 100K orders from the Brazilian e-commerce marketplace.

The dataset contains interconnected information about:

- Customers
- Orders
- Order Items
- Products
- Sellers
- Payments
- Reviews
- Geolocation
- Product Category Translation

The original dataset is not included in this repository because of its size. The project files and dashboard are provided separately.

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Microsoft Excel | Data analysis, PivotTables and dashboards |
| Power Query | Data cleaning and transformation |
| Power Pivot | Data modeling and relationships |
| DAX | Measures and analytical calculations |
| PivotTables | Aggregation and analysis |
| Data Visualization | Business dashboard development |

---

## 🧹 Data Cleaning & Transformation

The project included a full data-quality review rather than only removing null values.

Main steps included:

- Checking missing and blank values
- Detecting duplicate records
- Validating data types
- Cleaning text and encoding issues
- Standardizing category and location values
- Validating dates and timestamps
- Checking numeric and financial values
- Investigating invalid/negative values
- Checking referential integrity between related tables
- Creating useful analytical columns
- Preparing the data for the final model and dashboard

---

## 🧩 Data Model

The project uses a relational data model connecting the main business entities.

### Main Relationships

```text
Customers
    │
    └── Orders
          ├── Order Items ─── Products
          │        │
          │        └── Sellers
          │
          ├── Payments
          │
          └── Reviews

Category Translation ─── Products
```

This model allows the dashboard to analyze the same business from multiple perspectives while maintaining relationships between customers, orders, products, sellers, payments, and reviews.

---

## 📐 DAX Measures

Examples of the analytical measures used in the project include:

- **Total Orders**
- **Total Sales**
- **Average Order Value**
- **Average Review Score**
- **Total Products Sold**
- **Average Payment Installments**
- **Average Delivery Days**

These measures were used throughout the PivotTables and dashboard pages.

---

## 📊 Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Orders | 99,441 |
| Total Customers | 96,096 |
| Total Products Sold | 112,650 |
| Total Sales | 16,008,872.12 |
| Average Order Value | 160.99 |
| Average Review Score | 4.09 |
| Average Delivery Days | 12.50 |

> Sales is calculated from payment values, while product/category/seller sales analysis uses order-item price where appropriate.

---

## 📈 Key Insights

### Sales Performance

- Sales increased substantially from 2016 to 2017.
- November 2017 recorded a major monthly sales peak.
- The dataset becomes incomplete toward the end of 2018, so the final months should not be interpreted as a full-year decline.

### Product Categories

The leading categories by sales included:

1. Health & Beauty
2. Watches & Gifts
3. Bed, Bath & Table
4. Sports & Leisure
5. Computers & Accessories

### Geographic Performance

Sales were highly concentrated in several Brazilian states, with:

- São Paulo contributing approximately **38.3%** of order-item sales.
- Rio de Janeiro contributing approximately **13.4%**.
- Minas Gerais contributing approximately **11.7%**.

### Payments

Credit cards represented approximately **78.3%** of payment value, followed by boleto at approximately **17.9%**.

### Delivery

- **89.15%** of orders were delivered on time.
- **7.87%** were late.
- **2.98%** were not delivered.

Average delivery time was approximately **12.50 days**.

### Customer Satisfaction

- 5-star reviews represented approximately **57.8%** of reviews.
- 4–5 star reviews represented approximately **77.1%**.
- 1–2 star reviews represented approximately **14.7%**.

The analysis also showed a strong relationship between delivery status and review scores: on-time orders had a higher average review score than late or not-delivered orders.

---

## 🚚 Business Problems Identified

The analysis highlighted several areas for business attention:

- Delivery delays
- Lower satisfaction associated with delayed deliveries
- Geographic concentration of sales
- High freight costs in some product categories
- Seasonal sales fluctuations
- Dependence on specific payment methods

---

## 💡 Recommendations

Based on the analysis, potential business actions include:

- Monitor delayed orders and identify bottlenecks earlier.
- Improve coordination between sellers and logistics providers.
- Prepare inventory and logistics capacity for seasonal peaks.
- Analyze high-freight product categories to identify cost-saving opportunities.
- Monitor customer satisfaction by delivery performance.
- Investigate lower-volume geographic markets for future expansion.
- Maintain contingency plans for major logistics disruptions.

These recommendations are based on patterns observed in the dataset and are intended as business-analysis suggestions rather than causal conclusions.

---

## 🖥️ Dashboard

The final Excel dashboard is organized into four analytical pages:

### 1. Sales Overview
- Sales KPIs
- Sales trend
- Sales by category
- Top products
- Sales by state

### 2. Customers & Payments
- Customer KPIs
- Payment methods
- Installment categories
- Customers by state
- Payment analysis

### 3. Products & Sellers
- Top categories
- Top sellers
- Products sold
- Freight analysis

### 4. Delivery & Satisfaction
- Delivery status
- Average delivery time
- Review score distribution
- Delivery vs. customer satisfaction
- Geographic delivery performance

---

## 📁 Project Files

The repository contains the presentation, documentation, and dashboard screenshots.

The **full Excel dashboard workbook** is approximately 49 MB because it contains the Power Query/Power Pivot data model and PivotTable structures. It is therefore provided through an external file link rather than stored directly in this GitHub repository.

### 📊 Full Excel Dashboard

**[Open / Download the Final Excel Dashboard](PASTE_YOUR_EXCEL_FILE_LINK_HERE)**

> Replace the link above with the Google Drive / OneDrive / other sharing link for the final Excel workbook.

### 📑 Project Presentation

The PowerPoint presentation summarizes the project methodology, KPIs, findings, business problems, recommendations, and dashboard.

### 📄 Project Documentation

The project documentation contains the detailed cleaning, transformation, modeling, DAX, and analysis work.

---

## 📸 Dashboard Preview

Dashboard screenshots are included in the `Screenshots` folder to provide a quick visual overview of the final analysis.

---

## 📚 Data Source

**Olist Brazilian E-Commerce Public Dataset**

The dataset was originally published as a public Brazilian e-commerce dataset for analytical and educational use.

---

## 👩‍💻 Project Author

**Donia Khaled**

Computer Science / Medical Informatics Student  
Aspiring Data Analyst

### Skills Demonstrated

`Excel` · `Power Query` · `Power Pivot` · `DAX` · `Data Cleaning` · `Data Modeling` · `Data Visualization` · `Business Analysis`

---

## ⭐ Project Highlights

This project demonstrates an end-to-end workflow:

**Raw Data → Data Cleaning → Transformation → Data Modeling → DAX → Analysis → Dashboard → Business Insights → Recommendations**

