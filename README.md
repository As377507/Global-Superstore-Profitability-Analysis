# Global Superstore Profitability and Performance Analysis

## 🎯 Project Overview

This project utilizes **Power BI** to create an interactive, professional dashboard designed to provide actionable insights into the sales, profit, and operational efficiency of a global superstore chain (using the simulated `Global Superstore` dataset).

The primary goal is to shift focus from high-level revenue metrics to detailed **profitability analysis** to identify loss-making products and underperforming markets, guiding strategic business interventions.

---

## 📊 Key Performance Indicators (KPIs) & Insights

The dashboard is structured around key business questions to ensure data drives action.

| Insight | Visualization | Technical Implementation | Business Impact |
| :--- | :--- | :--- | :--- |
| **Financial Health** | **Profit Margin KPI** | Created using DAX: `Profit Margin = DIVIDE(SUM(Profit), SUM(Sales))`. Uses conditional formatting (Red/Green) to instantly alert if margin is below a target (e.g., 10%). | Provides context to raw profit numbers, indicating the true efficiency of sales. |
| **Actionable Profitability** | **Profit by Sub-Category Bar Chart** | Bars are conditionally formatted: **Red** for negative profit, **Green** for positive profit. | Pinpoints exact product lines (e.g., 'Tables', 'Binders') that must be addressed for pricing or cost reduction. |
| **Geographic Performance** | **Sales and Profit by Market Matrix** | Replaced complex map visual with a Matrix table using conditional formatting (Red/Green background) on the Profit column. | Quickly ranks global markets by performance, allowing management to prioritize resource allocation. |
| **Trend Analysis** | **Sales Trend Over Time** Line Chart | Shows monthly/quarterly sales trends, revealing seasonality and peak demand periods. | Supports forecasting and inventory planning. |

---

## 🛠️ Technical Details & Power BI Techniques

### Data Source
* **File:** `Global_Superstore2.csv` (Simulated Retail Data)
* **Key Fields:** `Sales`, `Profit`, `Order Date`, `Category`, `Sub-Category`, `Market`, `Region`.

### Key DAX Measure
The core of the analysis relies on the calculated Profit Margin:

```dax
Profit Margin = 
DIVIDE(
    SUM('Global_Superstore2'[Profit]), 
    SUM('Global_Superstore2'[Sales])
)
```

### Techniques Used
* **Conditional Formatting:** Applied rules to KPI cards and the Sub-Category Bar Chart to highlight performance deviations using color.
* **Professional Design:** Utilized a minimalist design (white background, clean fonts, consistent color palette) and removed unnecessary visual borders.

---
## 🔗 Deliverables
* **Dashboard Image:**
  ![Dashboard](screenshots/Sales_Report_screenshort.png)
* **Power BI Source File:** `Global_Superstore2.pbix`
* ![PowerBI File](File/Sales Report.pbix)
