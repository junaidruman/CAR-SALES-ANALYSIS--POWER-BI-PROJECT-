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

YTD Total Sales: $371.2M
Formula: SUM('Car Data'[Total Sales])
MTD Total Sales — $54.28M
Formula: CALCULATE(SUM('Car Data'[Total Sales]),DATESMTD('Calendar Table'[Date]))

YOY Growth in Total Sales: 23.6%
Formula: [Sales Difference]/[PTYD Total Sales]
Difference between YTD Sales and PTYD Sales: $70.8M
Formula: [YTD Car Sales]-[PTYD Car Sales]
Average Price Analysis:

YTD Average Price: $28.0k
Formula: TOTALYTD([Avg Price],'Calendar Table'[Date])
MTD Average Price: $28.26k
Formula: TOTALMTD([Avg Price],'Calendar Table'[Date])
YOY Growth in Average Price: -0.79%
Formula: [Avg Price Diff]/[PTYD Avg Price]
Difference between YTD Average Price and PTYD Average Price: $0.22k loss
Formula: [YTD Avg Price]-[PTYD Avg Price]
Cars Sold Metrics:

YTD Cars Sold: 13.3K
Formula: SUM('Car Data'[YTD Car Solds])
MTD Cars Sold: 1.92k
Formula: CALCULATE(SUM('Car Data'[MTD Cars Sold]), DATESMTD('Calendar Table'[Date]))
**YOY Growth in
Cars Sold:** 19.73% - Formula: car_data[Cars Sold Diff]/[YTD Car Solds]

Difference between YTD Cars Sold and PTYD Cars Sold: 3K
Formula: [YTD Car Solds]-[PTYD Car Solds]   
 


