# Superstore Insights Hub — E-Commerce Sales Analysis

## 🎯 Project Goal
End-to-end analysis of Superstore's retail transaction data (2014–2017) to uncover insights on sales performance, profitability, customer behavior, product performance, revenue trends, and order patterns — using Python, SQL, and Power BI.

---

## 📂 Dataset
- **Source:** Sample Superstore Dataset (Kaggle)
- **Size:** 9,994 rows, 21 columns
- **Time period:** January 2014 – December 2017
- **Key fields:** Order ID, Customer ID, Order Date, Ship Date, Segment, Region, Category, Sub-Category, Product Name, Sales, Quantity, Discount, Profit

---

## 🛠️ Tools Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn) — data cleaning, EDA, correlation analysis, revenue forecasting
- **MySQL** — query-based validation of KPIs and trends
- **Power BI** — interactive dashboard with dynamic filters

---

## 🧹 Data Cleaning
- Verified 0 missing values and 0 duplicate rows across all 9,994 records
- Converted `Order Date` and `Ship Date` to proper datetime format
- Standardized text fields (Category, Region) for consistent casing
- Validated no negative Sales or Quantity values; confirmed Discount range (0–80%) and Profit range (-$6,599.98 to $8,399.98) are legitimate business values

---

## 📊 Key KPIs

| Metric | Value |
|---|---|
| Total Sales | $2,297,200.86 |
| Total Profit | $286,397.02 |
| Total Orders | 5,009 |
| Average Order Value (AOV) | $458.61 |
| Profit Margin | 12.47% |

---

## 📈 Key Insights

1. **Technology leads in sales ($836K) and profit margin (17.4%)**, while Furniture generates comparable sales ($742K) but the lowest profit margin (2.5%) — driven by above-average discounting (17.4% avg. discount vs. 13.2% for Technology).

2. **Discounting hurts profit without boosting sales.** Discount vs. Profit correlation is **-0.22** (heavier discounts → lower profit), while Discount vs. Sales correlation is only **-0.03** (discounts barely move sales volume). This suggests discounting is eroding profitability without a meaningful sales payoff.

3. **The West region leads in both sales and profit**; Central shows the weakest profit relative to its sales volume, making it the region most worth investigating for cost or pricing issues.

4. **Order volume is unusually low on Wednesdays** — only 371 orders compared to 1,100–1,870 on every other weekday — a mid-week lull worth flagging for promotional timing.

5. **Revenue shows a consistent upward trend from 2014 to 2017**, with strong seasonal spikes every November/December, consistent with holiday shopping behavior.

6. **98.5% of customers made repeat purchases** over the 4-year period — note this reflects the long time span of the dataset rather than exceptional short-term loyalty.

---

## 🐍 Python Analysis
- Data cleaning and validation (Pandas)
- KPI computation (Total Sales, Profit, Orders, AOV, Profit Margin)
- Category/Region/Product/Segment performance breakdown
- Customer behavior analysis (repeat purchase rate)
- Order pattern analysis (day-of-week trends)
- Correlation analysis (Discount vs. Profit vs. Sales) with Seaborn heatmap
- Profit distribution analysis (Seaborn boxplot by Category)
- Revenue forecasting using 3-month moving average

## 🗄️ SQL Analysis (MySQL)
Queries written and validated against Python results:
- Top 10 selling products
- Sales and profit by category
- Monthly revenue trend
- Region-wise profit
- Average discount vs. average profit by category

## 📊 Power BI Dashboard — "Superstore Insights Hub"
- 5 KPI cards: Total Sales, Total Profit, Total Orders, AOV, Profit Margin
- Sales by Region (bar chart)
- Sales by Category (donut chart)
- Monthly Revenue Trend (line chart)
- Top 10 Products by Sales (bar chart)
- Profit by Sub-Category (bar chart)
- Sales by Segment (donut chart)
- Interactive filters (dropdown slicers): Region, Category, Order Date

---

## 📁 Project Structure
```
Ecommerce-Sales-Analysis/
├── Dataset/
│   ├── Superstore_Data.csv
│   └── Superstore_clean.csv
├── SQL Queries/
│   └── analysis.sql
├── Power BI Dashboard/
│   └── Superstore_Insights_Hub.pbix
├── Python Analysis/
│   └── analysis.ipynb
├── Screenshots/
│   ├── dashboard_overview.png
│   └── dashboard_filtered.png
└── README.md
```

---

## 🔑 Skills Demonstrated
Data Cleaning · Exploratory Data Analysis · Statistical Correlation Analysis · SQL Querying · Data Visualization · Dashboard Design · Business Insight Generation · Revenue Forecasting

---

## 👤 Author
[Your Name]
[Your LinkedIn] · [Your GitHub] · [Your Email]
