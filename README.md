# 🚗 Uber Trip Analysis – Power BI Case Study

An end-to-end **Uber Trip Analysis** project focused on analyzing large-scale trip data to uncover demand patterns, operational inefficiencies, and revenue-driving factors using **Power BI**.

---

## 📌 Project Overview

This project transforms raw trip-level data into actionable business insights supporting data-driven decisions related to pricing, driver allocation, and customer experience.

- **Dataset Period:** June 1, 2024 – June 30, 2024
- **Total Trips Analyzed:** 103,728
- **Tool:** Power BI (3-page interactive dashboard)

---

## 🎯 Business Objectives

- Analyze overall trip volume and revenue trends
- Identify peak demand hours and high-demand zones
- Understand customer payment preferences
- Evaluate trip distance and duration patterns
- Recommend optimization strategies for operations and pricing

---

## 📊 Key Metrics (Dashboard KPIs)

| Metric | Value |
|---|---|
| Total Bookings | 103.7K |
| Total Booking Amount | $1.6M |
| Avg Booking Value | $15.0 |
| Total Trip Distance | 349K miles |
| Avg Trip Distance | 3 miles |

---

## 🔍 Key Insights

### 💳 Payment Preferences
- **Uber Pay dominates** at 67.03% (70K trips)
- Cash accounts for 32.23% (33K trips)
- Amazon Pay & Google Pay minimal (0.17%)
- Digital payments strongly preferred — opportunity to phase out cash dependency

### 🌙 Day vs Night Trips
- **Day trips: 65.28%** (68K) vs Night trips: 34.72% (36K)
- Significant daytime demand — driver allocation should prioritize daytime shifts

### 🚗 Vehicle Type Performance
| Vehicle | Bookings | Revenue | Distance |
|---|---|---|---|
| UberX | 38,744 | $583,880 | 131,496 mi |
| Uber Comfort | 17,078 | $253,995 | 56,790 mi |
| Uber Black | 16,710 | $250,192 | 56,149 mi |
| UberXL | 16,698 | $249,424 | 55,721 mi |
| Uber Green | 14,498 | $216,181 | 48,778 mi |

- **UberX is the clear leader** — 37% of all bookings
- All vehicle types maintain consistent avg booking value of $15

### ⏰ Time-Based Demand
- **Peak hours: 12 PM – 6 PM** (afternoon surge)
- **Lowest demand: 2 AM – 5 AM**
- **Busiest day: Sunday (19.2K trips)**
- **Quietest day: Friday (9.3K trips)**
- Weekend demand significantly higher than weekdays

### 📍 Location Insights
- **Most frequent pickup:** Penn Station/Madison Sq West (4.5K)
- **Most frequent drop-off:** Upper East Side North (4.5K)
- **Farthest trip:** Lower East Side → Crown Heights North (144 miles)
- Top 5 locations concentrate around Manhattan hubs

---

## 🗂️ Dataset Description

- **Trip Details** – Trip-level info: distance, duration, fare, surge, vehicle, payment
- **Location Table** – Pickup and drop-off location mapping
- **Dashboard File** – Power BI report with all visuals and DAX measures

---

## 🧱 Data Preparation & Modeling

- Cleaned and standardized trip-level metrics
- Handled missing and inconsistent values
- Created active and inactive relationships for accurate pickup/drop-off analysis
- Built date and time attributes for hourly and daytime insights

---

## 🧮 Key DAX Measures

```dax
Total Booking Value = SUM(fare_amount + Surge Fee)

Total Bookings = COUNT('Trip Details'[Trip ID])

Avg Miles = AVERAGE('Trip Details'[trip_distance])

Avg Time =
AVERAGEX(
    TripData,
    DATEDIFF(Pickup, DropOff, MINUTE)
)
```

---

## 📋 Dashboard Pages

| Page | Description |
|---|---|
| Overview Analysis | KPIs, payment type, vehicle breakdown, location analysis |
| Time Analysis | Hourly trends, day-wise patterns, hour × day heatmap |
| Details | Raw trip-level data table |

---

## 💡 Optimization Strategies

- **Dynamic Dispatch** — Reposition drivers to Penn Station & Upper East Side during peak hours
- **Fare Normalization** — Apply balanced surge pricing on Sunday afternoons (peak demand)
- **Time-Based Optimization** — Align driver availability with 12 PM–6 PM peak window
- **Digital Payment Push** — Incentivize Uber Pay to reduce cash dependency
- **UberX Focus** — Prioritize UberX fleet expansion given dominant demand

---

## 🛠 Tech Stack

| Tool | Usage |
|---|---|
| Power BI | Data modeling, DAX, dashboard design |
| DAX | Custom KPIs and calculations |
| Excel | Raw data storage and preprocessing |
| GitHub | Version control and project hosting |

---

## 🚀 Project Deliverables

- Power BI Dashboard (`.pbix`)
- Trip Details Dataset (`.xlsx`)
- Location Mapping Dataset (`.xlsx`)

---

## 🔮 Future Enhancements

- Add predictive demand forecasting
- Integrate real-time trip data via API
- Enhance dashboard with drill-through analysis
- Extend analysis with customer segmentation

---

## 👤 Author

**Yash Jani**  
Data Analyst | Power BI | SQL | Machine Learning  
[GitHub: yashjani1997](https://github.com/yashjani1997)
