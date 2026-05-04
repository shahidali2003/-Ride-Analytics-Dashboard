# 🚖 Ride Analytics Dashboard (Power BI)

## 🔹 Overview

End-to-end ride analytics dashboard covering bookings, cancellations, revenue, ratings, and performance. Fully dynamic with slicers, drill-downs, and cross-filtering.

---

## 🔹 Key KPIs

* Total Bookings
* Total Cancellations
* Cancellation %
* Revenue Metrics (Total, Per KM, Momentum)
* Avg Distance / Total Distance
* Customer & Driver Ratings

---

## 🔹 Features

* 📅 **Dynamic Date Filter** (range slicer)
* 🚗 **Vehicle Type Filter**
* 💳 **Payment Category Filter**
* 📊 **Drill-down visuals** (Month → Day)
* 🔄 **Cross filtering across visuals**
* 📈 Trend analysis (Monthly, Weekly)
* 📉 Cancellation insights (Driver vs Customer reasons)

---

## 🔹 Pages Breakdown

1. **Homepage**

   * Navigation UI + branding

2. **Overall**

   * KPI cards + booking trends + status distribution

3. **Vehicle Report**

   * Vehicle-wise bookings, revenue, distance

4. **Revenue**

   * Revenue by tier, distance category, trend

5. **Cancellation**

   * Driver vs Customer cancellation analysis

6. **Rating**

   * Customer vs Driver rating comparison

7. **Summary**

   * Combined business snapshot

---

## 🔹 Data Pipeline

1. Raw dataset (ride bookings)
2. Data cleaning (Power Query)
3. Data modeling (relationships, measures)
4. DAX calculations (KPIs, % metrics)
5. Visualization (Power BI report)

---

## 🔹 Sample DAX

```DAX
Total Bookings = COUNT(rideBookings[Booking ID])

Total Cancelled = SUM(rideBookings[Count of cancellation Ride])

Cancellation % = 
DIVIDE([Total Cancelled], [Total Bookings], 0)
```

---

## 🔹 Tools Used

* Power BI
* Power Query
* DAX
* Excel / CSV dataset

---

## 🔹 Live Dashboard

(🔗 Add your Power BI publish link here)

---

## 🔹 Use Cases

* Ride-hailing business insights
* Operations monitoring
* Customer behavior analysis
* Revenue optimization

---

## 🔹 Author

Shahid Ali



## 🔄 Dashboard Workflow

1. **Data Source**

   * Ride booking dataset (Bookings, Revenue, Distance, Ratings)

2. **Data Cleaning (Power Query)**

   * Missing values handled
   * Data types fixed
   * Columns structured

3. **Data Modeling**

   * Fact table: rideBookings
   * Dimension: Date, Vehicle, Payment
   * Relationships created

4. **DAX Layer**

   * KPIs (Bookings, Revenue, Cancellation %)
   * Aggregations & calculated measures

5. **Visualization Layer**

   * KPI Cards
   * Pie charts (Booking status, cancellations)
   * Bar charts (Revenue, distance)
   * Line charts (Trends)

6. **Interactivity**

   * Slicers (Date, Vehicle, Payment)
   * Cross-filtering
   * Drill-down enabled

7. **UI/UX Layer**

   * Clean layout
   * Color-coded sections
   * Navigation buttons

8. **Publishing**

   * Published to Power BI Service
   * Shareable dashboard link

9. **End User Flow**

   * Select filters → View KPIs → Drill into insights → Take decisions
