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

### 🚗 SALES OVERVIEW


- **YTD Total Sales:** $371.2M  
  - **Formula:** `SUM('Car Data'[Total Sales])`

- **MTD Total Sales:** $54.28M  
  - **Formula:** `CALCULATE(SUM('Car Data'[Total Sales]), DATESMTD('Calendar Table'[Date]))`

- **YOY Growth in Total Sales:** 23.6%  
  - **Formula:** `[Sales Difference] / [PTYD Total Sales]`

- **Difference between YTD Sales and PTYD Sales:** $70.8M  
  - **Formula:** `[YTD Car Sales] - [PTYD Car Sales]`

### 💰 Average Price Analysis

- **YTD Average Price:** $28.0K  
  - **Formula:** `TOTALYTD([Avg Price], 'Calendar Table'[Date])`

- **MTD Average Price:** $28.26K  
  - **Formula:** `TOTALMTD([Avg Price], 'Calendar Table'[Date])`

- **YOY Growth in Average Price:** -0.79%  
  - **Formula:** `[Avg Price Diff] / [PTYD Avg Price]`

- **Difference between YTD Average Price and PTYD Average Price:** $0.22K loss  
  - **Formula:** `[YTD Avg Price] - [PTYD Avg Price]`

###🚘 Cars Sold Metrics

- **YTD Cars Sold:** 13.3K  
  - **Formula:** `SUM('Car Data'[YTD Car Solds])`

- **MTD Cars Sold:** 1.92K  
  - **Formula:** `CALCULATE(SUM('Car Data'[MTD Cars Sold]), DATESMTD('Calendar Table'[Date]))`

- **YOY Growth in Cars Sold:** 19.73%  
  - **Formula:** `car_data[Cars Sold Diff] / [YTD Car Solds]`

- **Difference between YTD Cars Sold and PTYD Cars Sold:** 3K  
  - **Formula:** `[YTD Car Solds] - [PTYD Car Solds]`

 
---

# 📋 DETAILED SALES GRID
Complete transaction-level sales data for deep analysis.

📷  
<img width="1204" height="672" alt="image" src="https://github.com/user-attachments/assets/3c8ce717-cc7c-4d57-ab1f-20eb85f6fb34" />


<img width="1206" height="676" alt="image" src="https://github.com/user-attachments/assets/f6df33dc-fd22-4628-bd3a-65367c945853" />


---

# 📈 KEY BUSINESS INSIGHTS

- 📈 **23.59% YoY Sales Growth** generating **$371.2M**
- 💰 Avg car price dropped **0.79%**
- 🏆 Austin & Janesville are top-performing regions
- 📅 Peak sales in **Week 36 & Week 47**
- 🚘 Car sales volume increased **19.73% YoY**
- 🎨 Pale White = top color
- 🚙 SUVs & Hatchbacks = best body styles
- 🏭 Chevrolet, Ford & Dodge contribute **18% of total sales**
- ⚙️ Automatic transmission outsold manual
- 🔧 DOHC engines outsold OHC

---

# ⚠️ AREAS REQUIRING ATTENTION

- Improve pricing strategy to reverse **0.79% price drop**
- Boost low-performing regions: **Middletown & Pasco**
- Strengthen **Q1 & Q2 sales strategies**
- Increase sales for **Jaguar & Hyundai**

---

# 🏁 CONCLUSION
This Car Sales Analytics Dashboard offers a comprehensive view of the dealership's performance in 2023, providing valuable insights into sales trends, KPIs, and areas for improvement. With a clear visualization of key metrics and actionable analysis, this dashboard serves as a powerful tool for making informed decisions and driving growth in the competitive automotive market.


