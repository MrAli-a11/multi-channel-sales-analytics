# Multi-Channel Sales Analytics Dashboard

An end-to-end Business Intelligence project that integrates sales and inventory data from multiple platforms into a centralized reporting solution using Google BigQuery, SQL, and Power BI.

## 🛠 Tech Stack

- SQL
- Google BigQuery
- Power BI
- DAX
- Power BI Service
- Microsoft Excel
- Google Sheets

## 📌 Project Overview

This project is an end-to-end Business Intelligence solution built to analyze multi-channel sales and inventory data. Data is collected from multiple business sources, transformed using Google BigQuery, and visualized in Power BI to support daily business reporting and decision-making.

The dashboard provides insights into sales performance, product performance, category trends, city-wise sales, platform comparison, and key business KPIs through an interactive reporting interface.

## 🏗️ Data Architecture

The project follows a **3-layer data warehouse architecture** to ensure clean, scalable, and reliable reporting.

```text
Raw Layer
│
├── petpooja_raw
├── production_raw
├── shopify_raw
├── sku_master_raw
└── vendor_inward_raw

        │
        ▼

Clean Layer
│
├── petpooja_clean
├── production_clean
├── shopify_clean
├── sku_master_clean
└── vendor_inward_clean

        │
        ▼

Reporting Layer (Gold)
│
├── dim_sku_master
├── fact_sales
├── master_inflow
└── master_sales

        │
        ▼

Power BI Desktop
        │
        ▼

Power BI Service


```

> **Note:** Data transformation and reporting layers were built using a combination of SQL Views and Tables in Google BigQuery to create a scalable reporting pipeline.

## ✨ Features

- End-to-end ETL pipeline using Google BigQuery
- 3-layer data warehouse architecture (Raw → Clean → Gold)
- Multi-channel sales integration (Shopify, Petpooja, Swiggy, Zomato & Offline)
- Interactive Power BI dashboard
- KPI tracking (Sales, Orders, Quantity, AOV)
- Product & Category performance analysis
- Platform-wise sales comparison
- City-wise sales analysis
- DAX measures for dynamic calculations
- Published to Power BI Service

## 📊 Business Problem

Business data was spread across multiple platforms including Shopify, Petpooja, Swiggy, Zomato, Production, and Vendor records. Manual reporting was time-consuming, error-prone, and lacked a centralized view for decision-making.

This project solves the problem by integrating data into a centralized BigQuery warehouse and providing an interactive Power BI dashboard for daily business insights.

## 🚀 Key Outcomes

- Centralized reporting across multiple business platforms
- Reduced manual reporting effort
- Improved data consistency using a structured data warehouse
- Enabled faster business decision-making through interactive dashboards
- Automated KPI reporting using Power BI and BigQuery

<img width="1775" height="874" alt="image" src="https://github.com/user-attachments/assets/ca949039-4ae6-4a3c-832b-3634ec97b4dd" />

## 📂 Repository Structure

```text
multi-channel-sales-analytics/
│
├── dashboard/
│   └── Sales_Dashboard.pbix
│
├── screenshots/
│   └── dashboard-overview.png
│
├── sql/
│   ├── create_tables.sql
│   ├── create_views.sql
│   └── analysis_queries.sql
│
├── docs/
│   └── architecture.md
│
└── README.md
```

## 🔮 Future Improvements

- Implement scheduled data refresh
- Add inventory forecasting dashboard
- Integrate Python ETL pipeline
- Add Row-Level Security (RLS)
- Build executive and operational dashboards

## 👨‍💻 Author

**Hasnain Ali**

- LinkedIn: www.linkedin.com/in/mr-ali123
- Email: mrali9132@gmail.com

