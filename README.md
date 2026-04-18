## Project Overview
This project showcases an end-to-end **Business Intelligence solution** built using **Microsoft Power BI** on the Adventure Works dataset.

The dashboard is designed to deliver **actionable insights** across:
- Sales & Revenue Performance
- Customer Behavior
- Product Analysis
- Regional Distribution

---

## Key Business Questions Solved
✔ What is the overall revenue, profit, and order trend?  
✔ Which products and categories drive maximum sales?  
✔ Who are the top customers contributing to revenue?  
✔ How does performance vary across regions?  
✔ What is the return rate and its impact?  

---

## Dashboard Structure

### Executive Dashboard
- Revenue: **₹24.9M**
- Profit: **₹10.5M**
- Orders: **25.2K**
- Return Rate: **2.2%**
- Revenue trend analysis over time
- Category-wise order distribution
- Top 10 products by revenue & returns

---

### Map Analysis
- Global sales distribution (USA, Canada, Europe, Australia)
- Region-based filtering:
  - Europe
  - North America
  - Pacific
- Interactive geographic insights

---

### Product Detail Page
- Selected Product Analysis (Dynamic)
- Monthly Orders vs Target
- Revenue vs Target
- Profit vs Target
- Price Adjustment simulation
- Profit comparison (Adjusted vs Actual)

---

### Customer Detail Page
- Unique Customers: **17.4K**
- Revenue per Customer: **₹1.4K**
- Top 100 Customers ranking
- Top Customer Highlight:
  - **Mr. Maurice Shan**
- Orders & Revenue breakdown
- Customer segmentation:
  - Income Level
  - Occupation

---

## Key Features
✨ Interactive slicers & filters  
✨ Drill-down & drill-through capabilities  
✨ Dynamic KPI cards  
✨ Clean dark-themed UI  
✨ Scenario analysis (Price Adjustment)  
✨ Top N analysis (Customers & Products)  

---

## DAX Measures Used
DAX
Total Revenue = SUM(Sales[Sales Amount])

Total Profit = SUM(Sales[Profit])

Total Orders = COUNT(Sales[Order ID])

Return Rate = DIVIDE([Total Returns], [Total Orders], 0)

Revenue Per Customer = 
DIVIDE([Total Revenue], DISTINCTCOUNT(Customer[Customer ID]))

Top Customer Rank = 
RANKX(ALL(Customer), [Total Revenue], , DESC)

### Data Model
-Fact Table: Sales
-Dimension Tables:
-Customer
-Product
-Geography
-Date

* Optimized using Star Schema Design *

## Design Highlights
-Dark theme with teal accents (high contrast readability)
-KPI-focused layout
-Consistent visual hierarchy
-Minimal clutter, maximum insight

## Key Insights

-📌 Accessories generate the highest orders
-📌 Tires & Tubes are the most ordered product types
-📌 Shorts have the highest return rate
-📌 Revenue shows consistent growth trend post-2021
-📌 Top customers contribute significantly to total revenue

## Tools & Technologies
-Microsoft Power BI
-Power Query (ETL)
-DAX (Data Analysis Expressions)
-Data Modeling

## How to Use
-Download the .pbix file
-Open in Power BI Desktop
-Navigate through pages using tabs
-Apply filters & interact with visuals
## Future Improvements
-Add forecasting (AI visuals)
-Implement Row-Level Security (RLS)
-Connect to live data sources
-Enhance mobile layout

##👤 Author

**Amit Kumar ( Data Analyst)**
