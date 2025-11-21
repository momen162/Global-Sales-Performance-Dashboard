# Global Sales Performance Dashboard

![Dashboard_Preview](https://github.com/user-attachments/assets/ff32a542-a92b-4060-942c-d8f235414549)


## 🚀 Introduction
This project is an advanced, interactive dashboard that transforms over **60,000+ raw transaction records** into actionable business insights.

This project demonstrates a complete data workflow: starting with raw CSV data, performing **ETL (Extract, Transform, Load)** in Power Query to build a **Star Schema** data model, and developing a dynamic "Dark Mode" executive dashboard. The final result allows stakeholders to analyze performance across regions, products, and customer demographics in real-time.

**Demo:** 

## 🛠️ Excel Skills Demonstrated
✔️ **Power Query** for data cleaning, unpivoting, and text manipulation (splitting columns).<br>
✔️ **Data Modeling (Star Schema)** to organize data into 1 Fact Table and 4 Dimension Tables.<br>
✔️ **Data Normalization** to reduce redundancy and improve query performance.<br>
✔️ **Pivot Tables** for data aggregation and multi-dimensional analysis.<br>
✔️ **Slicers & Interactivity** to filter data by Year, Region, and Category instantly.

## 📚 Table of Contents
1. [Problem Statement](#problem-statement)
2. [Data Transformation & Modeling](#data-transformation--modeling)
3. [Analysis and Visualization](#analysis-and-visualization)
4. [Conclusion & Recommendations](#conclusion--recommendations)

## Problem Statement
This dashboard was built to answer key strategic questions for the executive team:<br>
💰 **Financial Health:** What is our total revenue, profit, and profit margin efficiency?<br>
🌍 **Geography:** Which regions (and channels like Online vs. Store) are driving growth?<br>
👥 **Demographics:** Who is our ideal customer profile (Age, Gender)?<br>
🏆 **Product Strategy:** Which brands and categories yield the highest ROI?<br>
📅 **Seasonality:** What are the weekly and monthly trends we need to prepare for?<br>

**Features:** Order Date, Store Country, Product Category, Brand, Customer DOB, Quantity, Price, Cost.

## Data Transformation and Modeling
The backbone of this dashboard is a robust **Star Schema** model created to optimize performance:

1. **Data Cleaning (Power Query):**
   - Imported raw transaction data.
   - Fixed data types and handled missing values.
   - **Text Transformation:** Solved complex text wrapping issues (e.g., "Music, Movies and Audio Books") using Power Query text replacement functions.
2. **Normalization:**
   - Split the flat file into **5 distinct tables**:
     - `Fact_Sales` (Transactions)
     - `Dim_Customer` (Demographics)
     - `Dim_Product` (Category, Brand)
     - `Dim_Store` (Region)
     - `Dim_Date` (Time Intelligence)
3. **Feature Engineering:**
   - **Age Groups:** Calculated customer age from DOB and grouped them into bins (e.g., "60+", "20-30") to find the target audience.
   - **Profit Margin %:** Created a calculated measure `(Revenue - Cost) / Revenue` to track efficiency.
   - **Weekly Patterns:** Extracted "Day of Week" to identify peak trading days.

## 🎨 Key Performance Indicators (KPIs)
- **Total Revenue:** $55.8M
- **Total Profit:** $32.7M
- **Profit Margin:** 58.6%
- **Total Orders:** 26,326
- **Top Region:** United States

## Analysis and Visualization

### 1. Sales Volume vs. Margin Efficiency (Combo Chart)
<img width="722" height="452" alt="image" src="https://github.com/user-attachments/assets/e7532014-e714-4dce-908b-a113a7a67298" />

**Insight:** While **"Computers"** drive the highest sales volume, the **"Audio & Media"** category delivers the highest profit margin (>60%). This suggests a strategy of volume vs. value balance.

### 2. Top 3 Brands by Sales (Pie Chart)
<img width="722" height="452" alt="image" src="https://github.com/user-attachments/assets/101f51f7-dbe3-4e7a-8789-2fe959fac576" />

**Insight:** The market is heavily dominated by two key suppliers: **Adventure Works** and **Contoso**. These two brands alone account for a significant portion of total revenue, indicating a need to maintain strong supplier relations with them.

### 3. Monthly Sales Trends (Line chart)
<img width="722" height="452" alt="image" src="https://github.com/user-attachments/assets/611f412e-daef-4ff3-b601-fd9ce3f9787c" />

### 4. Global Regional Performance (Donut Chart)
<img width="721" height="452" alt="image" src="https://github.com/user-attachments/assets/470ef3ac-a331-4de1-aedc-cf393d0a49de" />

**Insight:** The **United States** is the top-performing physical region, but **"Online"** sales have emerged as the second-largest "region," outperforming major countries like the UK and Germany combined.

## Conclusion and Recommendations

### 🎯 Conclusion
The analysis reveals a highly profitable business ($32.7M Profit) driven by a mature customer base (60+) and specific high-value brands (Adventure Works). While the US market is strong, the "Online" channel is a critical growth engine.

### 💡 Recommendations
1.  **Target the 60+ Demographic:** Shift marketing imagery and campaigns to resonate with the mature audience that is driving $18M+ in sales, rather than targeting Gen Z.
2.  **Supplier Strategy:** Negotiate exclusive deals or volume discounts with **Adventure Works** and **Contoso** as they are the anchors of the business.
3.  **Product Mix:** Promote "Audio" products in bundles with "Computers" to attach high-margin items to high-volume purchases.
