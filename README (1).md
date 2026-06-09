# 🛍️ Vrinda Store — Annual Sales Data Analysis (2022)

> An end-to-end Excel-based data analysis project covering data cleaning, processing, and an interactive dashboard to help Vrinda Store understand their 2022 sales performance and grow in 2023.

---

## 📌 Project Overview

Vrinda Store is an Indian online fashion retailer selling categories like Kurtas, Sets, Sarees, Western Dresses, and Tops across major e-commerce platforms — Amazon, Flipkart, Myntra, Meesho, Ajio, and Nalli.

The store owner wanted a single, consolidated annual report to answer key business questions and identify opportunities for growth. This project delivers that through a clean dataset and an interactive Excel dashboard.

---

## 🎯 Business Questions Answered

The dashboard was built to answer the following questions raised by the store owner:

1. **Sales vs. Orders Comparison** — A single combo chart showing monthly sales amount and order count side by side.
2. **Highest Sales Month** — Which month saw the peak in both revenue and number of orders?
3. **Men vs. Women Purchasing** — Who bought more in 2022?
4. **Order Status Breakdown** — What percentage of orders were Delivered, Cancelled, Returned, or Refunded?
5. **Top 10 States by Sales** — Which states contributed the most to revenue?
6. **Age vs. Gender Analysis** — How do different age groups (Teenager, Adult, Senior) break down by gender in terms of order count?
7. **Best Performing Sales Channel** — Which platform (Amazon, Myntra, Flipkart, etc.) drove maximum sales?
8. **Highest Selling Category** — Which product category (Kurta, Set, Saree, etc.) sold the most?

---

## 🗂️ Dataset Description

**File:** `Vrinda_Store_Data_Analysis.xlsx`  
**Sheet:** `Vrinda Store`  
**Total Columns:** 21

| Column | Description |
|---|---|
| `index` | Row identifier |
| `Order ID` | Unique order number |
| `Cust ID` | Customer ID |
| `Gender` | Customer gender (Men / Women) |
| `Age` | Customer age |
| `Age Group` | Derived: Teenager / Adult / Senior |
| `Date` | Order date |
| `Month` | Derived month name |
| `Status` | Order status (Delivered, Cancelled, Returned, Refunded) |
| `Channel` | Sales platform (Amazon, Myntra, Flipkart, Meesho, Ajio, Nalli, Others) |
| `SKU` | Product code |
| `Category` | Product category (kurta, Set, Saree, Top, Western Dress) |
| `Size` | Product size (XS to 6XL) |
| `Qty` | Quantity ordered |
| `currency` | INR |
| `Amount` | Order value in INR |
| `ship-city` | Delivery city |
| `ship-state` | Delivery state |
| `ship-postal-code` | PIN code |
| `ship-country` | Country (IN) |
| `B2B` | Whether order is B2B (TRUE/FALSE) |

---

## 🧹 Data Cleaning

The following cleaning steps were performed before analysis:

- **Standardized Gender column** — inconsistent entries like `M`, `Men`, `man` were unified to `Men`; similarly for Women.
- **Standardized Qty column** — entries like `One`, `1` were normalized to numeric values.
- **Handled blank/null values** — checked all columns for missing data and handled appropriately.
- **Corrected data types** — ensured date columns were in proper date format; amount and qty as numbers.
- **Removed duplicate entries** — checked for and removed any duplicate Order IDs.

---

## ⚙️ Data Processing

New derived columns were added to support analysis:

- **Age Group** — Categorized `Age` into:
  - `Teenager` (≤ 25)
  - `Adult` (26–60)
  - `Senior` (> 60)
- **Month** — Extracted month name from the `Date` column for time-series analysis.

---

## 📊 Dashboard & Analysis

The final Excel dashboard includes the following charts:

| Chart | Type | Insight |
|---|---|---|
| Sales vs. Orders by Month | Combo Chart (Bar + Line) | Monthly trend of revenue and volume |
| Gender Split | Pie / Bar Chart | Women vs. Men purchase share |
| Order Status | Pie Chart | Delivery success rate |
| Top 10 States | Bar Chart | Geographic revenue contribution |
| Age vs. Gender | Grouped Bar Chart | Demographic breakdown of buyers |
| Sales by Channel | Bar / Pie Chart | Best performing platform |
| Sales by Category | Bar Chart | Top product categories |

Slicers/filters are connected to all charts for dynamic exploration by Month, Channel, and Category.

---

## 🔍 Key Insights (Sample)

- **Women** account for significantly more purchases than men (~65%+).
- **Adult women** (26–60) are the dominant buyer demographic.
- **Amazon, Myntra, and Flipkart** are the top 3 sales channels.
- **Maharashtra, Karnataka, and Uttar Pradesh** lead in state-wise sales.
- **Sets and Kurtas** are the highest-selling product categories.
- Order delivery rate is high, with cancellations and returns being a small fraction.

---

## 🛠️ Tools Used

- **Microsoft Excel** — Data cleaning, processing, pivot tables, charts, and dashboard
- **Pivot Tables** — For aggregating data across dimensions (month, state, channel, gender, age group)
- **Slicers** — For interactive filtering on the dashboard

---

## 📁 Project Structure

```
Vrinda-Store-Analysis/
│
├── Vrinda_Store_Data_Analysis.xlsx   # Main file with raw data, cleaned data & dashboard
└── README.md                          # Project documentation (this file)
```

---

## 🚀 How to Use

1. Open `Vrinda_Store_Data_Analysis.xlsx` in Microsoft Excel.
2. Navigate to the **Dashboard** sheet.
3. Use the **Slicers** (Month, Channel, Category) to filter charts interactively.
4. Refer to individual sheets for raw data and pivot table breakdowns.

---

## 👤 Author

**Parth** — B.E. Computer Science (AI/ML), APSIT, University of Mumbai  
Semester 6 | Data Analytics & Visualization Project

---

*This project was built as part of a data analytics learning exercise to simulate a real-world business dashboard use case.*
