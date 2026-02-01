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
![Transformation](images/transformation.png)

---

# 🔗 DATA MODELLING
Established a **one-to-many relationship** between:

**Calendar Table ➝ Car Data**

📷  
![Data Model](images/datamodel.png)

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
