# 🚖 OLA Ride Booking Analysis

> **End-to-end data analytics project analyzing ride bookings, revenue, cancellations, vehicle performance, and customer/driver ratings for July 2024.**

---

## 📌 Project Overview

This project analyzes **103,024 ride-booking records for July 2024** to understand booking performance, revenue patterns, cancellation behavior, vehicle utilization, and service quality.

The analysis follows a complete data analytics workflow using **Excel, SQL, and Power BI**, transforming raw ride-booking data into business-focused insights and an interactive dashboard.

> **Note:** The dataset is a project/synthetic ride-booking dataset created for analytics practice and is **not official OLA proprietary data**.

---

## 🎯 Business Objectives

The analysis focuses on answering key business questions:

* How are ride bookings performing over time?
* What proportion of bookings are successful or cancelled?
* Which vehicle types contribute most to ride distance?
* Which payment methods generate the highest booking value?
* Who are the highest-value customers?
* Why are customers and drivers cancelling rides?
* How do customer and driver ratings compare?
* Where can operational efficiency and customer experience be improved?

---

## 🛠️ Tools & Technologies

* **Excel** — Data preparation and initial analysis
* **SQL** — Data querying and business analysis
* **Power BI** — Interactive dashboard and data visualization

---

# 📊 Key Business Insights

## 1. Overall Booking Performance

The dataset contains **103,024 total bookings** during July 2024.

* **63,967 bookings (62.09%)** were successful.
* **18,434 bookings (17.89%)** were cancelled by drivers.
* **10,499 bookings (10.19%)** were cancelled by customers.
* **10,124 bookings (9.83%)** resulted in the driver not being found.

This shows that although successful rides form the majority of bookings, cancellations and unsuccessful booking outcomes represent a significant opportunity for operational improvement.

---

## 2. 🚗 Vehicle Performance

The dashboard compares vehicle categories based on ride activity and distance.

The analysis covers:

* Auto
* Bike
* eBike
* Mini
* Prime Sedan
* Prime Plus
* Prime SUV

This helps identify differences in vehicle utilization and supports better fleet planning and vehicle allocation decisions.

---

## 3. 💰 Revenue & Payment Analysis

The revenue analysis evaluates booking value across different payment methods:

* Cash
* UPI
* Credit Card
* Debit Card

The dashboard also identifies the **Top 5 customers by total booking value**.

The five highest-value customers generated a combined booking value of **₹32,612**, with the highest individual customer contributing **₹8,025**.

This analysis can help businesses understand payment preferences and identify high-value customers for retention initiatives.

---

## 4. ❌ Customer Cancellation Analysis

Customer cancellations were analyzed by cancellation reason.

The leading reasons were:

1. **Driver not moving towards pickup location** — 3.18K (30.24%)
2. **Driver asked customer to cancel** — 2.67K (25.43%)
3. **Change of plans** — 2.08K (19.82%)
4. **AC not working** — 1.57K (14.93%)
5. **Wrong address** — 1.01K (9.57%)

The largest customer-side cancellation issue is related to the driver not moving toward the pickup location, indicating a potential driver responsiveness and pickup-experience problem.

---

## 5. 👨‍✈️ Driver Cancellation Analysis

Driver cancellations were also analyzed by reason.

The major reasons were:

* **Personal & car-related issues** — 6.54K (35.49%)
* **Customer-related issues** — 5.41K (29.36%)
* **Customer coughing/sick** — 3.65K
* **More passengers than permitted** — 2.83K

The results indicate that both vehicle/driver-related issues and customer-related issues contribute significantly to cancellations.

---

## 6. ⭐ Ratings & Service Quality

The dashboard compares:

* Driver ratings
* Customer ratings

Ratings remain close to the **4.0 level** across the analyzed period, indicating relatively consistent service experiences between customers and drivers.

This metric can be monitored alongside cancellations to identify whether service-quality issues are associated with unsuccessful rides.

---

# 💡 Business Recommendations

### 1. Reduce Driver-Side Cancellations

Monitor vehicle availability and driver readiness before accepting rides, particularly for reasons related to personal or vehicle issues.

### 2. Improve Pickup Reliability

The high number of cancellations caused by drivers not moving toward pickup suggests an opportunity to improve driver response and pickup monitoring.

### 3. Strengthen Customer Retention

The highest-value customers can be targeted through loyalty programs, personalized offers, and repeat-ride incentives.

### 4. Encourage Digital Payments

Understanding payment-method preferences can help optimize digital payment adoption and improve transaction convenience.

### 5. Monitor Vehicle Performance

Vehicle-level ride-distance analysis can support better fleet allocation and help identify high-performing vehicle categories.

---

# 📈 Dashboard Sections

The Power BI dashboard is organized into five analytical views:

### Overall

* Ride Volume Over Time
* Booking Status Breakdown

### Vehicle Type

* Vehicle Type performance
* Ride Distance comparison

### Revenue

* Revenue by Payment Method
* Top 5 Customers by Booking Value
* Daily Ride Distance

### Cancellation

* Customer Cancellation Reasons
* Driver Cancellation Reasons
* Cancellation Rate

### Ratings

* Driver Ratings
* Customer Ratings

---

# 🧮 SQL Analysis

SQL was used to answer business questions such as:

* Retrieve successful bookings
* Calculate average ride distance by vehicle type
* Count customer cancellations
* Identify top customers
* Analyze driver cancellation reasons
* Find minimum and maximum driver ratings
* Identify UPI bookings
* Calculate average customer ratings
* Calculate successful booking value
* Retrieve incomplete rides and their reasons

The complete SQL script is available in:

`sql/Ola_Project.sql`

---

# 📁 Project Structure

```text
ola_ride_booking_analysis/
│
├── README.md
│
├── data/
│   └── Bookings-100000-Rows.xlsx
│
├── sql/
│   └── Ola_Business_Problems.sql
│
├── powerbi/
│   └── Ola_Ride_Booking_Analysis.pbix
│
├── dashboard/
│   └── OLA_Ride_Booking_Dashboard.pdf
│
└── documentation/
    └── OLA-Data-Analyst-Project-1.pdf
```

---

# 🔄 Analytics Workflow

**Raw Dataset → Data Preparation → SQL Analysis → Business Insights → Power BI Dashboard**

The project demonstrates how raw booking data can be transformed into meaningful information for understanding operational performance, customer behavior, revenue, and service quality.

---

## ✅ Conclusion

The OLA Ride Booking Analysis provides a consolidated view of **booking performance, revenue, cancellations, vehicle utilization, and service quality**.

The analysis highlights cancellation behavior as one of the key operational areas requiring attention while also identifying opportunities around **customer retention, payment adoption, fleet optimization, and pickup reliability**.

The project demonstrates an end-to-end approach to turning raw ride-booking data into **business-focused insights that can support operational and management decisions**.
