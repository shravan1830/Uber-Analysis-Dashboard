# Uber Trip Analysis Dashboard

## 1. Project Title / Headline

**Uber Trip Analysis: Interactive Business Intelligence Dashboard**
A dynamic Power BI dashboard designed to analyze Uber ride data, uncover booking trends, revenue patterns, trip behavior, and location-based insights through interactive visualizations.

---

## 2. Short Description / Purpose

The Uber Trip Analysis Dashboard provides a comprehensive overview of ride bookings, revenue generation, trip distances, and time-based patterns. It is built to help analysts, operations teams, and decision-makers quickly understand customer behavior, operational performance, and geographical demand trends using data-driven insights.

---

## 3. Tech Stack

The dashboard was developed using the following tools and technologies:

* **Power BI Desktop** – Primary platform for building interactive visualizations and reports
* **Power Query** – Data cleaning, transformation, and preparation layer
* **DAX (Data Analysis Expressions)** – Used for calculated measures such as total bookings, average trip distance, and booking value metrics
* **Data Modeling** – Fact and dimension tables structured to enable slicing by date, city, vehicle type, and trip attributes
* **File Formats**

  * `.pbit` – Power BI template file for development
  * `.png` – Dashboard screenshots for documentation and previews

---

## 4. Data Source

**Source:** Uber trip dataset (simulated / analytical dataset for BI purposes)

The dataset contains detailed ride-level information, including:

* Booking dates and times
* City and location details (pickup & drop-off)
* Trip distance and duration
* Booking value and payment methods
* Vehicle types (UberX, UberXL, Uber Comfort, Uber Black, Uber Green)

The data is structured to support time-series analysis, location intelligence, and vehicle performance comparisons.

---

## 5. Features / Highlights

### Business Problem

Ride-hailing platforms generate massive volumes of trip data, but raw data alone does not provide actionable insights. Stakeholders need an intuitive way to monitor bookings, revenue, trip efficiency, and customer preferences across time, locations, and vehicle categories.

### Goal of the Dashboard

The primary goal of this dashboard is to:

* Track overall business performance (bookings, revenue, distance, time)
* Identify trends by day, location, and vehicle type
* Understand customer payment preferences
* Support operational and strategic decision-making using visual analytics

### Key Questions Answered

* How many total bookings and how much revenue is generated?
* What is the average booking value, trip distance, and trip duration?
* How do bookings fluctuate day by day?
* Which payment methods and trip times (day/night) generate more revenue?
* Which locations have the highest pickup and drop-off demand?
* Which vehicle types perform best in terms of bookings and revenue?

### Walkthrough of Key Visuals

* **KPI Cards (Top Section)**
  Displays high-level metrics such as total bookings, total booking value, average booking value, total trip distance, average trip distance, and average trip time.

* **Time & Value Analysis**
  Toggle-based visuals to analyze:

  * Total Bookings
  * Total Booking Value
  * Total Trip Distance

* **Payment Type & Trip Timing Analysis (Donut Charts)**
  Visual breakdown of booking value by:

  * Payment method (Uber Pay, Cash, Amazon Pay, Google Pay)
  * Trip timing (Day vs Night trips)

* **Daily Booking Trend (Line Chart)**
  Shows booking volume trends across days, helping identify peak and low-demand periods.

* **Location Analysis**
  Highlights:

  * Most frequent pickup point
  * Most frequent drop-off point
  * Farthest recorded trip

* **Vehicle Type Analysis (Table & Bar Charts)**
  Comparison of vehicle categories based on:

  * Total bookings
  * Total booking value
  * Average booking value
  * Total trip distance

---

### Business Impact & Insights

* **Operational Optimization**: Helps operations teams identify high-demand locations and peak booking times.
* **Revenue Strategy**: Reveals which vehicle types and payment methods contribute most to revenue.
* **Fleet Planning**: Assists in aligning vehicle availability with customer demand by location.
* **Customer Behavior Analysis**: Provides insights into trip patterns, distances, and preferences.
* **Executive Reporting**: Enables leadership to track KPIs at a glance through an intuitive interface.

---

## 6. DAX Measures (Key Examples)

Below are sample DAX measures used in the dashboard to calculate KPIs and enable dynamic analysis. These measures highlight the use of aggregation, averages, and time-based calculations.

### 1. Total Bookings

Counts the total number of Uber trips (bookings) recorded in the dataset.

```DAX
Total Bookings = 
COUNT('Uber Trips'[Booking_ID])
```

**Usage:** Displayed in KPI cards and used across visuals to analyze demand trends by date, city, and vehicle type.

---

### 2. Total Booking Value

Calculates the total revenue generated from all Uber trips.

```DAX
Total Booking Value = 
SUM('Uber Trips'[Booking_Value])
```

**Usage:** Drives revenue analysis across payment types, trip timing (day/night), vehicle categories, and locations.

---

### 3. Average Trip Distance

Computes the average distance per trip to understand customer travel behavior.

```DAX
Avg Trip Distance = 
AVERAGE('Uber Trips'[Trip_Distance_Miles])
```

**Usage:** Used in KPI cards and vehicle type analysis to compare trip efficiency and distance patterns.

---

### Optional Advanced Measure (Time Intelligence)

Calculates average trip duration in minutes.

```DAX
Avg Trip Time (Minutes) = 
AVERAGE('Uber Trips'[Trip_Duration_Minutes])
```

**Usage:** Helps evaluate operational efficiency and customer ride experience.

---

## 7. Screenshots / Demo

You can view the dashboard screenshot using the link below:

👉 **Snapshot of Uber Dashboard:**
[https://github.com/shravan1830/Uber-Analysis-Dashboard/blob/main/Snapshot%20of%20Uber%20Dashboard.png](https://github.com/shravan1830/Uber-Analysis-Dashboard/blob/main/Snapshot%20of%20Uber%20Dashboard.png)

---<img width="1327" height="751" alt="Snapshot of Uber Dashboard" src="https://github.com/user-attachments/assets/2a4ee836-f401-4b47-ae48-5e1eabbabbb6" />

> *Note:* This image represents the main overview page of the Uber Trip Analysis Power BI dashboard.

## 8. Author

**Developed by:** Shravan Kalzunkar

If you find this project useful, feel free to ⭐ the repository and explore more Power BI analytics projects.
