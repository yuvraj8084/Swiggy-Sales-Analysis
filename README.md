# Swiggy Sales Analysis

Exploratory data analysis of **1.97 lakh+ Swiggy food-order records** (Jan to Aug 2025) using Python, to track sales KPIs and uncover trends across time, location and food category.

---

## Project Overview

This project analyzes Swiggy sales data covering **28 states, 28 cities and 993 restaurants**. The goal is to understand how revenue is distributed across regions, days, months and food types (veg vs non-veg), and to summarize business performance through key KPIs.

## Dataset

- **File:** `swiggy_data.xlsx`
- **Records:** 197,430
- **Period:** January to August 2025
- **Columns (10):**

| Column | Description |
|---|---|
| State | State of the restaurant |
| City | City of the restaurant |
| Order Date | Date of the order |
| Restaurant Name | Name of the restaurant |
| Location | Area within the city |
| Category | Food category of the restaurant |
| Dish Name | Name of the dish |
| Price (INR) | Price of the dish |
| Rating | Customer rating |
| Rating Count | Number of ratings received |

## Tools & Libraries

- **Python**
- **Pandas, NumPy** for data handling and analysis
- **Matplotlib, Plotly** for static and interactive visualizations
- **Jupyter Notebook**

## Analysis Performed

1. Data inspection (shape, data types, missing values, duplicates)
2. Date feature engineering (month, week, day of week, quarter)
3. KPI calculation: Total Sales, Average Order Value, Average Rating, Total Rating Count
4. Monthly, weekly and day-wise sales trends
5. Veg vs Non-Veg classification from dish names and revenue comparison
6. State-wise and city-wise revenue analysis (Top 5 cities)
7. Quarterly performance summary (sales, records, rating)

## Key KPIs

| KPI | Value |
|---|---|
| Total Sales | ₹5.30 Cr |
| Average Order Value | ₹268.5 |
| Average Rating | 4.34 |
| Total Records | 1.97 lakh+ |
| Total Rating Count | 55.9 lakh+ |

## Key Insights

- **Veg dishes contribute about 65% of revenue**, while non-veg contributes about 35%.
- **Bengaluru (Karnataka) is the top market**, with about ₹54.6 lakh in sales (about 10% of total).
- **Top 5 cities by revenue:** Bengaluru, Lucknow, Hyderabad, Mumbai and New Delhi, together contributing about one-third of total sales.
- **Saturday is the best-performing day** (about 14.7% of sales), but the gap between days is small, so demand is fairly consistent across the week.
- **Monthly sales are stable** at roughly ₹62 to ₹68 lakh, with January being the highest.

## Notes & Limitations

- **Veg/Non-Veg split is approximate.** Dishes were classified using keyword matching on dish names (e.g., chicken, egg, fish), so a few dishes may be misclassified.
- **Q3 (2025) is a partial quarter.** The data ends on 31 Aug, so Q3 contains only two months and looks lower in sales. This is not a real decline.
- **Records, not order IDs.** The dataset has no order ID column, so "orders" here means dish-level records.
- Each state has one city in this dataset, so state-wise and city-wise rankings are identical.

## Project Structure

```
swiggy-sales-analysis/
│
├── Swiggy_Sales_Analysis.ipynb   # Main analysis notebook
├── swiggy_data.xlsx              # Dataset
└── README.md
```

## How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/YOUR-USERNAME/swiggy-sales-analysis.git
   cd swiggy-sales-analysis
   ```
2. Install the required libraries
   ```bash
   pip install pandas numpy matplotlib plotly openpyxl jupyter
   ```
3. Open the notebook
   ```bash
   jupyter notebook Swiggy_Sales_Analysis.ipynb
   ```

## Future Improvements

- Build an interactive **Power BI dashboard** on this data
- Add a **SQL** analysis of the same dataset
- Improve veg/non-veg classification with a more complete dish list

## Author

**YOUR NAME**
[LinkedIn](https://linkedin.com/in/YOUR-LINKEDIN) | [GitHub](https://github.com/YOUR-GITHUB)
