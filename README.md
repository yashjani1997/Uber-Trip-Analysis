# 🚗 Uber Trip Analysis (Power BI Case Study)

## 📌 Project Overview
This project is an end-to-end Uber Trip Analysis focused on analyzing large-scale trip data to uncover demand patterns, operational inefficiencies, and revenue-driving factors using Power BI.

The objective is to transform raw trip-level data into actionable business insights that support data-driven decision-making related to pricing, driver allocation, and customer experience.

---

## 🎯 Business Objectives
- Analyze overall trip volume and revenue trends
- Identify peak demand hours and high-demand zones
- Understand customer payment preferences
- Evaluate trip distance and duration patterns
- Recommend optimization strategies for operations and pricing

---

## 🗂️ Dataset Description
The analysis is based on the following datasets:

- Trip Details – Trip-level information including distance, duration, fare, and surge
- Location Table – Pickup and drop-off location mapping
- Dashboard File – Power BI report containing all visuals and measures

---

## 🧱 Data Preparation & Modeling
- Cleaned and standardized trip-level metrics
- Handled missing and inconsistent values
- Created active and inactive relationships for accurate pickup and drop-off analysis
- Built date and time attributes to enable hourly and daytime insights

This data model ensures accurate aggregations and reliable analysis.

---

## 🛠️ Tools & Technologies Used
- Power BI – Data modeling, DAX measures, dashboard design
- DAX – Custom KPIs and calculations
- Excel – Raw data storage and preprocessing
- GitHub – Version control and project hosting

---

## 🧮 Key DAX Measures
    Total Booking Value = SUM(fare_amount + Surge Fee)

    Total Bookings = COUNT('Trip Details'[Trip ID])

    Avg Miles = AVERAGE('Trip Details'[trip_distance])

    Avg Time =
    AVERAGEX(
        TripData,
        DATEDIFF(Pickup, DropOff, MINUTE)
    )

---

## 📊 Dashboard Highlights
The Power BI dashboard provides insights into:

- Total trips and revenue performance
- Hourly and daytime demand patterns
- Pickup and drop-off location analysis
- Payment method distribution
- Trip distance and duration trends

The dashboard is designed with a clean, business-focused layout for fast insight discovery.

---

## 💡 Optimization Strategies
Based on the analysis, the following strategies were identified:

- Dynamic Dispatch – Repositioning drivers to high-demand zones using demand heatmaps
- Fare Normalization – Applying balanced surge pricing during peak hours
- Time-Based Demand Optimization – Aligning driver availability with peak demand windows
- Zone-Level Performance Analysis – Identifying high-demand and low-efficiency locations
- Payment Preference Optimization – Supporting seamless digital payment experiences

---

## 🚀 Project Deliverables
- Power BI Dashboard (.pbix)
- Trip Details Dataset (.xlsx)
- Location Mapping Dataset (.xlsx)
- Interactive HTML project page (deployed on Vercel)


---

## 🔮 Future Enhancements
- Add predictive demand forecasting
- Integrate real-time trip data
- Enhance dashboard with drill-through analysis
- Extend analysis with customer segmentation

---

## 👤 Author
Yash Jani  
Data Analyst | Power BI | SQL | Machine Learning  
GitHub: https://github.com/yashjani1997
