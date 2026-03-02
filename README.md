# 🏡 Luxury Housing Sales Analysis

### End-to-End Data Analytics Project (Python + SQL + Power BI)

---

## 📌 Project Overview

The **Luxury Housing Sales Analysis** project is an end-to-end data analytics solution developed to analyze luxury property sales performance and market trends.

This project transforms raw housing sales data into actionable business insights using **Python for data processing**, **SQL for database management**, and **Power BI for interactive visualization**.

The goal is to help stakeholders understand:

* Property sales performance
* Market trends
* Revenue distribution
* Geographic performance
* Top-performing locations

---

## 🎯 Business Objective

The dashboard answers important real-estate business questions:

1. Sales trend across quarters
2. Revenue performance by location
3. Top-performing housing markets
4. Property price distribution
5. Geographic sales insights
6. Market demand analysis
7. Booking/Sales growth trends
8. Location-wise revenue contribution
9. Market comparison analysis
10. Top luxury housing performers

---

## 🧩 Project Architecture

```
CSV Dataset
     ↓
Python Data Cleaning
     ↓
Data Transformation
     ↓
SQL Database Creation
     ↓
Power BI Connection
     ↓
Interactive Dashboard
```

---

## ⚙️ Step-by-Step Execution

---

## ✅ Step 1 — Data Collection

The dataset was provided in **CSV format** containing luxury housing sales information.

Sample columns include:

* Property Name
* City
* Micro Market
* Sale Date
* Property Price
* Total Revenue
* Sales Count

---

## ✅ Step 2 — Loading Data Using Python

The CSV dataset was loaded into Python for preprocessing.

Purpose:

* Handle raw dataset
* Prepare structured data for analysis

---

## ✅ Step 3 — Data Cleaning Using Python

Data preprocessing steps performed:

* Removed duplicate records
* Handled missing values
* Standardized column names
* Converted date formats
* Corrected data types
* Cleaned inconsistent entries

Outcome:
✔ Clean and analysis-ready dataset

---

## ✅ Step 4 — Data Transformation & Modeling

New analytical columns were created for reporting.

```

This improves dashboard filtering and trend analysis.

---

## ✅ Step 5 — Database Connection & Table Creation Using Python

After cleaning the dataset, a database connection was established and tables were created directly using Python.

Database Details:

* **Database Name:** `luxuary_housing`
* **Table Name:** `housing_sales`

Example:

```python
import sqlalchemy

engine = sqlalchemy.create_engine(
"mysql+pymysql://username:password@localhost/luxuary_housing"
)

df.to_sql(
    "housing_sales",
    engine,
    index=False,
    if_exists="replace"
)
```

Result:

* Database created
* Table generated automatically
* Structured storage enabled for BI reporting

---

## ✅ Step 6 — Connecting SQL Database to Power BI

Steps followed:

1. Open Power BI Desktop
2. Click **Get Data**
3. Select **SQL Server / MySQL**
4. Enter database details
5. Select table **housing_sales**
6. Load dataset

---

## ✅ Step 7 — Data Modeling in Power BI

Performed inside Power BI:

* Data validation
* Column formatting
* KPI measure creation using DAX

Example Measures:

``` DAX
Total Revenue = SUM(housing_sales[Revenue])

Total Sales = COUNT(housing_sales[Property_ID])
```

---

## ✅ Step 8 — Dashboard Development

Interactive dashboards were created to analyze housing sales performance.

### Key Visualizations

* Market Trend Line Chart
* Revenue Analysis
* Geographic Sales Map
* Property Performance
* Quarterly Sales Trend
* Top Performers Analysis

---

## 📊 Dashboard Pages

### 1️⃣ Executive Summary

Key KPIs:

* Total Revenue
* Total Properties Sold
* Average Property Price
* Top Performing Market

---

### 2️⃣ Market Trend Analysis

Shows quarterly sales growth across micro markets.

Visualization:

* Line Chart

---

### 3️⃣ Revenue Insights

Analyzes revenue contribution by:

* City
* Market
* Property Type

---

### 4️⃣ Geographic Insights

Map visualization displaying regional sales performance.

---

### 5️⃣ Top Performers

Top 5 luxury housing markets based on revenue.

---

## 📈 Key Business Insights

* Certain micro markets generate higher luxury property revenue.
* Sales trends vary across quarters, indicating seasonal demand.
* High-value cities dominate luxury housing sales.
* Geographic analysis helps identify investment hotspots.
* Data-driven insights support pricing and expansion strategies.

---

## 🛠 Tools & Technologies Used

| Tool     | Purpose                    |
| -------- | -------------------------- |
| Python   | Data Cleaning & Processing |
| Pandas   | Data Manipulation          |
| SQL      | Database Management        |
| Power BI | Dashboard Visualization    |
| DAX      | Business Calculations      |

---

## 🚀 Skills Demonstrated

* Data Cleaning using Python
* SQL Database Creation
* Data Modeling
* Business Intelligence Reporting
* Dashboard Development
* Data Visualization
* Business Insight Generation

---

## 📂 Repository Structure

```
Luxury-Housing-Sales-Analysis
│
├── data/
│   └── housing_sales.csv
│
├── python/
│   └── data_cleaning.ipynb
│
├── sql/
│   └── database_setup.sql
│
├── powerbi/
│   └── dashboard.pbix
│
└── README.md
```
**
Author
Malaviga Ravi
Aspiring Data Analyst/Data Scientist
Skills: Python, SQL, Data Visualization, BI Dashboards**
