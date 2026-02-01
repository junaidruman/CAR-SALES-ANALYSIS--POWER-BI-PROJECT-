# 🚗 CAR SALES ANALYTICS DASHBOARD  
## 📊 Power BI Project

---

# 📌 PROJECT OVERVIEW
Developed a dynamic and interactive **Car Sales Dashboard** using Power BI for a leading car dealership.  
Provides **real-time KPI insights** for data-driven decision-making.

---

# 🧹 DATA CLEANING & TRANSFORMATION
- Corrected data quality issues (spelling mistakes, inconsistencies)
- Used **Transform Data** for data type corrections
- Created a **Calendar Table** for YTD, MTD, YOY analysis
- Extracted **Week, Month, Year** using DAX

📷  
<img width="1857" height="785" alt="image" src="https://github.com/user-attachments/assets/e1facef0-835b-483c-8af8-5afcc5f970da" />

---

# 🔗 DATA MODELLING
Established a **one-to-many relationship** between:

**Calendar Table ➝ Car Data**

📷  
<img width="1427" height="617" alt="image" src="https://github.com/user-attachments/assets/61610296-3fb8-4932-8604-7585bc3e4fdf" />


---

# 🧮 DATA PREPARATION
- Built DAX measures for KPIs  
- Designed visual indicators with **color logic for profit/loss**

---

# 📊 KPI DASHBOARD METRICS

## 🚗 SALES OVERVIEW

**YTD Total Sales — $371.2M**
```DAX
SUM('Car Data'[Total Sales])
MTD Total Sales — $54.28M

CALCULATE(SUM('Car Data'[Total Sales]), DATESMTD('Calendar Table'[Date]))
YOY Growth in Total Sales — 23.6%

[Sales Difference] / [PTYD Total Sales]
YTD vs PTYD Sales Difference — $70.8M

[YTD Car Sales] - [PTYD Car Sales]
💰 AVERAGE PRICE ANALYSIS
YTD Average Price — $28.0K

TOTALYTD([Avg Price], 'Calendar Table'[Date])
MTD Average Price — $28.26K

TOTALMTD([Avg Price], 'Calendar Table'[Date])
YOY Growth in Avg Price — -0.79%

[Avg Price Diff] / [PTYD Avg Price]
YTD vs PTYD Avg Price Difference — $0.22K Loss

[YTD Avg Price] - [PTYD Avg Price]
🚘 CARS SOLD METRICS
YTD Cars Sold — 13.3K

SUM('Car Data'[YTD Car Solds])
MTD Cars Sold — 1.92K

CALCULATE(SUM('Car Data'[MTD Cars Sold]), DATESMTD('Calendar Table'[Date]))
YOY Growth in Cars Sold — 19.73%

car_data[Cars Sold Diff] / [YTD Car Solds]
YTD vs PTYD Cars Sold Difference — 3K

[YTD Car Solds] - [PTYD Car Solds]
📋 DETAILED SALES GRID
Complete transaction-level sales data for deep analysis.

📷


📈 KEY BUSINESS INSIGHTS
📈 23.59% YoY Sales Growth generating $371.2M

💰 Avg car price dropped 0.79%

🏆 Austin & Janesville are top-performing regions

📅 Peak sales in Week 36 & Week 47

🚘 Car sales volume increased 19.73% YoY

🎨 Pale White = top color

🚙 SUVs & Hatchbacks = best body styles

🏭 Chevrolet, Ford & Dodge = 18% of total sales

⚙️ Automatic > Manual transmission

🔧 DOHC engines outsold OHC

⚠️ AREAS REQUIRING ATTENTION
Improve pricing strategy to reverse 0.79% price drop

Boost low-performing regions: Middletown & Pasco

Strengthen Q1 & Q2 sales strategies

Increase sales for Jaguar & Hyundai

🏁 CONCLUSION
This dashboard delivers a complete performance view of dealership operations, combining KPIs, trends, and insights to support strategic decision-making and revenue growth.
