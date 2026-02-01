🚗 Car Sales Analytics Dashboard – Power BI
📌 Overview

Developed a dynamic and interactive Car Sales Dashboard using Microsoft Power BI for a leading car dealership.
The dashboard provides real-time insights into key performance indicators (KPIs) to support data-driven decision-making and performance monitoring.

🧹 Data Cleaning & Transformation

Corrected data quality issues (e.g., spelling mistakes)

Used Power BI Transform Data for data type corrections

Created a Calendar Table for YTD, MTD, and YOY analysis

Extracted Week, Month, and Year from Date using DAX

📷 Data Transformation View


🔗 Data Modelling

Built a one-to-many relationship between:

Calendar Table → Car Data

📷 Data Model


🧮 Data Preparation

Created DAX measures for KPI calculations

Designed KPI indicators using color logic for profit vs loss

📊 KPI Dashboard Metrics
🚗 Sales Overview

YTD Total Sales: $371.2M

SUM('Car Data'[Total Sales])


MTD Total Sales: $54.28M

CALCULATE(SUM('Car Data'[Total Sales]), DATESMTD('Calendar Table'[Date]))


YOY Growth in Total Sales: 23.6%

[Sales Difference] / [PTYD Total Sales]


Difference between YTD Sales and PTYD Sales: $70.8M

[YTD Car Sales] - [PTYD Car Sales]

💰 Average Price Analysis

YTD Average Price: $28.0K

TOTALYTD([Avg Price], 'Calendar Table'[Date])


MTD Average Price: $28.26K

TOTALMTD([Avg Price], 'Calendar Table'[Date])


YOY Growth in Average Price: -0.79%

[Avg Price Diff] / [PTYD Avg Price]


Difference between YTD Avg Price and PTYD Avg Price: $0.22K loss

[YTD Avg Price] - [PTYD Avg Price]

🚘 Cars Sold Metrics

YTD Cars Sold: 13.3K

SUM('Car Data'[YTD Car Solds])


MTD Cars Sold: 1.92K

CALCULATE(SUM('Car Data'[MTD Cars Sold]), DATESMTD('Calendar Table'[Date]))


YOY Growth in Cars Sold: 19.73%

car_data[Cars Sold Diff] / [YTD Car Solds]


Difference between YTD and PTYD Cars Sold: 3K

[YTD Car Solds] - [PTYD Car Solds]

📋 Detailed Sales Grid

Comprehensive grid displaying all individual car sales transactions for deep-dive analysis.

📷




📈 Key Business Insights

📈 23.59% YTD sales growth compared to 2022, generating $371.2M revenue

💰 Average car price decreased by 0.79%, highlighting pricing optimization opportunities

🏆 Austin led in total sales, followed by Janesville

📅 Peak sales weeks: Week 36 (September) and Week 47

🚘 Car sales volume increased 19.73% YoY

🎨 Pale White was the top-selling color

🚙 SUVs and Hatchbacks dominated body style sales

🏭 Chevrolet, Ford, and Dodge contributed nearly 18% of total sales

⚙️ Automatic transmission outsold manual

🔧 DOHC engines outsold OHC engines

⚠️ Areas Requiring Attention

Address 0.79% drop in average price to improve revenue

Improve sales in Middletown and Pasco regions

Strengthen Q1 & Q2 strategies to match later quarters

Boost performance for Jaguar and Hyundai (each <1% of sales)

🏁 Conclusion

This dashboard provides a complete performance overview of the dealership’s 2023 operations.
By combining interactive visuals, KPI tracking, and actionable insights, it enables smarter decisions and strategic growth in a competitive automotive market.
