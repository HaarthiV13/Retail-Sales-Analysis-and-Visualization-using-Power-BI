# Walmart Sales Analysis & Power BI Dashboard

## Project Overview

This project analyzes Walmart weekly sales data to **understand sales trends, store performance, and the impact of holidays and economic factors**. The analysis includes **data cleaning, exploration, visualization in Python**, and an **interactive Power BI dashboard** for business insights.

**Dataset:** Walmart Sales Forecasting (Kaggle)
**Tools Used:** Python (pandas, matplotlib, seaborn), Power BI Desktop

## Problem Statement

Walmart generates huge amounts of sales data across multiple stores. However, raw data alone does not provide actionable insights. The challenge is to **identify sales trends, top-performing stores, and the effect of holidays and external factors on sales**.

The goal is to **clean the dataset, explore patterns, visualize key insights, and build a dashboard** to support data-driven decision making.

## Workflow

### 1️⃣ Data Cleaning

* Fixed missing values in numerical columns (Temperature, Fuel Price, CPI, Unemployment).
* Converted `Date` column to proper datetime format.
* Created new time-based columns: `Year`, `Month`.
* Removed duplicates and handled outliers where needed.

### 2️⃣ Data Exploration (EDA)

* Analyzed **total weekly sales trend** over time.
* Identified **Top 10 stores** with highest average weekly sales.
* Compared **holiday vs non-holiday sales**.
* Studied **top months and seasonal sales trends**.
* Checked **correlation** between economic factors (Fuel Price, CPI, Unemployment) and sales.

### 3️⃣ Visualization (Python)

* **Line Chart:** Sales trend over time.
* **Bar Charts:** Top stores and top months.
* **Boxplot:** Holiday vs Non-Holiday sales.
* **Heatmap:** Correlation between sales and economic factors.

### 4️⃣ Power BI Dashboard

* KPI Cards: Total Sales, Average Weekly Sales, Total Stores, Total Months.
* Line Chart: Weekly Sales over time.
* Bar Chart: Top 10 Stores by Sales.
* Column Chart: Top 10 Months by Sales.
* Donut Chart: Holiday vs Non-Holiday sales.
* Scatter Plot: Relationship between Fuel Price and Sales.
* Filters: Year, Store

## Key Insights (Example)

* Sales peak during holiday weeks (Thanksgiving, Christmas).
* Some stores consistently outperform others.
* Certain months show strong seasonal trends in sales.
* Economic factors (Fuel Price, CPI, Unemployment) show weak-to-moderate correlation with sales.

## Folder Structure

```
walmart-sales-project/
│─ data/
│   └─ walmart.csv                # Original dataset from Kaggle
│─ notebooks/
│   └─ 01-clean-eda.ipynb        # Python notebook for cleaning & visualization
│─ outputs/
│   └─ walmart_cleaned.csv        # Cleaned dataset for Power BI
│─ powerbi/
│   └─ walmart_dashboard.pbix     # Power BI dashboard file
│─ README.md                      # Project overview
```

## How to Run

1. Download `walmart.csv` from Kaggle and place it in the `data/` folder.
2. Open `01-clean-eda.ipynb` in Jupyter Notebook and run all cells to perform cleaning and visualizations.
3. The cleaned dataset will be saved as `outputs/walmart_cleaned.csv`.
4. Open Power BI Desktop → Get Data → Import `walmart_cleaned.csv`.
5. Build visuals as described in the workflow.

## Skills & Tools Demonstrated

* Data Cleaning & Preprocessing (Python, pandas)
* Exploratory Data Analysis (Python, matplotlib, seaborn)
* Data Visualization & Storytelling
* Interactive Dashboard Creation (Power BI)
* Basic Time-Series & Seasonal Analysis
