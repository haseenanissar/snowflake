# 🌨️ Snowflake Data Warehouse Project: S3 to Snowflake Integration with Power BI

## 🚀 Project Overview

This project demonstrates a complete cloud-based ETL pipeline where raw data stored in **Amazon S3** is ingested into **Snowflake**, modeled using **star and snowflake schemas**, and visualized through **Power BI** dashboards. It uses **Snowpipe** for continuous data loading and includes staging, transformation, and dimensional modeling best practices.

---

## 📦 Tech Stack

| Layer           | Tool / Technology                     |
|----------------|----------------------------------------|
| Storage         | Amazon S3                              |
| Ingestion       | Snowpipe                               |
| Data Warehouse  | Snowflake                              |
| Modeling        | Star Schema & Snowflake Schema         |
| BI / Reporting  | Power BI                                |
| Orchestration   | (Optional) Apache Airflow               |
| Transformation  | SQL (Snowflake)                        |

---

## 📁 Project Structure

```bash
snowflake-etl-s3-to-powerbi/
├── sql/
│   ├── create_staging_tables.sql
│   ├── create_snowpipe.sql
│   ├── create_star_schema.sql
│   ├── create_snowflake_schema.sql
│   └── transformations.sql
├── s3_sample_data/
│   └── customer_orders.csv
├── powerbi/
│   └── PowerBI_Dashboard.pbix
├── docs/
│   ├── architecture_diagram.png
│   └── data_flow.md
├── README.md
└── .gitignore



Key Features
✅ S3 to Snowflake Integration
Data is loaded directly from Amazon S3 into Snowflake using external stages and file formats.

✅ Staging Layer
Raw data is ingested into staging tables for validation and cleanup.

✅ Automated Loading via Snowpipe
Snowpipe enables real-time/near-real-time ingestion from S3 using event notifications or manual triggers.

✅ Data Modeling

Star Schema: For performance-optimized reporting

Snowflake Schema: For normalized, scalable data storage

✅ Integration with Power BI
Dashboards built on modeled data for business analysis and insights.


