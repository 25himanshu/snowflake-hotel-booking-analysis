# ❄️ Snowflake Hotel Booking Analysis

### Transforming Raw Hotel Booking Data into Business Insights Using Snowflake SQL

## 📌 Project Overview

This project focuses on analyzing hotel booking data using Snowflake SQL. It implements a structured data processing workflow to load raw CSV data, clean and transform records, and generate analytical tables for business insights.

The project follows a **Medallion Architecture (Bronze, Silver, and Gold layers)** to organize data processing and prepare clean, analytics-ready datasets.

## 🎯 Project Objectives

- Load raw hotel booking data into Snowflake.
- Build a structured data warehouse using Medallion Architecture.
- Perform data cleaning and transformation using SQL.
- Analyze hotel bookings, revenue, booking status, and customer information.
- Create aggregated datasets to support dashboard reporting.

## 🛠️ Tech Stack

- **Cloud Data Platform:** Snowflake
- **Query Language:** SQL
- **Dataset:** CSV
- **Data Architecture:** Medallion Architecture
- **Data Processing:** Snowflake SQL
- **Analysis:** Aggregations, filtering, grouping, and sorting

## 🏗️ Data Architecture

The project follows a three-layer data architecture:

### 🥉 Bronze Layer – Raw Data

- Created the `HOTEL_DB` database.
- Configured CSV file format and Snowflake stage.
- Created the `BRONZE_HOTEL_BOOKING` table.
- Loaded raw booking records using `COPY INTO`.

### 🥈 Silver Layer – Cleaned Data

- Created the `SILVER_HOTEL_BOOKINGS` table.
- Cleaned customer names and hotel city values.
- Validated and standardized email addresses.
- Converted date fields into proper DATE format.
- Converted booking amounts into numeric values.
- Standardized booking status values.
- Filtered invalid booking dates.

### 🥇 Gold Layer – Analytics-Ready Data

Created analytical tables for business reporting:

- `GOLD_AGG_DAILY_BOOKING` – Daily booking counts and revenue.
- `GOLD_AGG_HOTEL_CITY_SALES` – Revenue analysis by hotel city.
- `GOLD_BOOKING_CLEAN` – Cleaned booking dataset for analysis.

## 📊 Business Analysis & KPIs

The project includes SQL queries to calculate:

- Average Booking Value
- Total Guests
- Total Bookings
- Total Revenue
- Daily Booking Trends
- Daily Revenue Trends
- Top 5 Cities by Revenue
- Bookings by Status
- Bookings by Room Type

## 📂 Project Structure

```text
snowflake-hotel-booking-analysis/
│
├── hotel_bookings_raw.csv
│
├── Processing.sql
│
├── Dashboard.sql
│
└── README.md
```

## ⚙️ Implementation Workflow

1. Create the Snowflake database.
2. Configure the CSV file format.
3. Create a Snowflake stage.
4. Create the Bronze table and load raw CSV data.
5. Perform data quality checks.
6. Transform and clean records into the Silver layer.
7. Create Gold analytical tables.
8. Execute KPI and business analysis queries.

## 💡 Key Learnings

- Working with Snowflake databases, tables, stages, and file formats.
- Loading CSV datasets using `COPY INTO`.
- Implementing Bronze, Silver, and Gold data layers.
- Performing data cleaning and transformation using SQL.
- Handling missing values, invalid dates, and inconsistent records.
- Building aggregated datasets for business reporting.
- Writing analytical SQL queries using GROUP BY, ORDER BY, SUM, AVG, and COUNT.

## 🚀 Future Enhancements

- Build an interactive Power BI dashboard.
- Automate data ingestion and transformation.
- Implement incremental data loading.
- Add advanced SQL analytics and window functions.
- Introduce data quality monitoring.

## 👨‍💻 Author

**Himanshu Khade**

- GitHub: [25himanshu](https://github.com/25himanshu)
- LinkedIn: [Himanshu Khade](https://www.linkedin.com/in/himanshu-khade-070209251/)

---

⭐ If you find this project useful, consider giving it a star!
