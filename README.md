# Retail Sales & Profit Dashboard (Excel & Tableau)

## Overview

This project analyzes retail profit performance by **product category**, **sub-category**, **region** and **time**.  
I built an interactive Tableau dashboard on top of an Excel data model to answer a simple business question:

> Which products and regions drive profit, and how does profit evolve over time?

The dashboard is designed for a non-technical business user to explore performance and spot opportunities.

---

## Dataset

- **Source:** [Product Sales Dataset (2023–2024)](https://www.kaggle.com/datasets/yashyennewar/product-sales-dataset-2023-2024) – Kaggle  
- **Grain:** One row per order line  
- **Main fields:**
  - `Order_Date`
  - `Region` (Centre, East, South, West)
  - `Category` (Accessories, Clothing & Apparel, Electronics, Home & Furniture)
  - `Sub_Category` (Bags, Bedding, Footwear, Furniture, Home Appliances, etc.)
  - `Profit`

---

## Business Questions

1. Which **categories** and **sub-categories** generate the highest profit?
2. Which **regions** are the most and least profitable?
3. How does **monthly profit** evolve over the 2023–2024 period?
4. Are there clear **seasonal peaks** or drops in profit across regions?

---

## Data Preparation (Excel)

I used Excel to prepare the data before visualising it in Tableau:

- Checked for missing values and inconsistent data types in the raw file.
- Aggregated metrics with **PivotTables**:
  - Profit by *Category*
  - Profit by *Region*
  - Profit by *Sub-Category*
- Calculated base KPIs such as:
  - Total Profit  
  - Number of Orders  
  - Average Profit per Order

The cleaned Excel file is then used as the single data source in Tableau.

---

## Dashboard (Tableau)

The Tableau workbook contains the following key views:

- **Category Profit**  
  Stacked bar chart showing profit by *Category*, split by *Region*.

- **Sub-Category Profit**  
  Bar chart comparing profit across sub-categories (Bags, Bedding, Footwear, Furniture, Home Appliances, Kitchenware, Laptops, Smartphones, Storage, etc.).

- **Profit by Region**  
  Bar chart showing total profit for each region (Centre, East, South, West).

- **Monthly Profit Trend by Region**  
  Line chart of monthly profit from **Jan 2023 to Dec 2024**, coloured by region to reveal seasonal patterns.

Interactive filters allow the user to slice results by category, region and date.

---

## Key Insights

- **Home & Furniture** is the most profitable category overall, followed by **Clothing & Apparel** and **Electronics**, while **Accessories** contributes the least profit.
- Within Home & Furniture, sub-categories like **Bedding**, **Kitchenware** and **Storage** stand out as top profit drivers.
- The **East** region generates the highest total profit, while the **South** region clearly lags behind the others.
- Monthly profit shows strong peaks around **November 2023** and **November 2024** across all regions, suggesting seasonal campaigns or holiday demand.
- Profit in the **South** region is consistently below the other regions throughout the period, indicating a potential opportunity to review pricing, assortment or marketing in that region.
