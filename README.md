# SQL-Data-Warehouse-Project
Building Model Data warehouse with ETL Processes and Star Schema

🏗️ Data Warehouse Architecture – Medallion Framework (Bronze / Silver / Gold)
📡 Data Sources

This project ingests enterprise data from two key operational platforms:

Source	Description
CRM	Contains customer interactions, sales funnel data, and relationship management information.
ERP	Includes finance, inventory, transactions, and operational business functions.

These raw data streams are ingested into the DWH as the starting point of the pipeline.

💾 Medallion Layer Structure

🟤 Bronze Layer – Raw Ingestion

Full-load ingestion only (no incremental processing).

Loads raw CRM and ERP data as-is.

Ensures traceability and source integrity.

⚪ Silver Layer – Transformation

Applies basic cleaning, standardization, and structure alignment.

Harmonizes CRM and ERP schemas.

Prepares clean, reliable data for reporting and analytics.


🟡 Gold Layer – Business-Ready Layer


Designed specifically for BI and business analytics needs.

Uses a Star Schema data modeling approach:

Fact tables for transactional/business measurement data (e.g., sales, bookings, transactions).

Dimension tables for descriptive attributes (e.g., customers, products, dates).

Optimized for:


Power BI dashboard performance

Ad-hoc SQL analytical queries

Fast query execution and simplified data navigation.


📊 Analytics & Consumption

Designed to support Power BI, self-service analytics, and ad hoc queries.

Allows business users and analysts to explore integrated CRM and ERP insights.

Method	How It Uses the Gold Layer

Power BI Dashboards	Connects to the Star Schema model to generate KPIs, 

visuals, and performance dashboards.

Ad-hoc SQL Queries	Analysts query fact and dimension tables directly for deeper insight and data exploration.

✔ Gold layer delivers clean, curated, business-aligned data in a scalable and high-performance structure.


📂 Repository Contents
Folder	Description
/docs	Architecture documentation, data flow, design choices
/scripts	ETL/ELT logic and pipeline scripts
/datasets	Sample data for implementation/testing
/tests	Validation scripts for ingestion and transformation


🚀 Key Highlights

✔ Built using a Data Architect approach for scalability

✔ Implements Medallion architecture best practices

✔ Data extracted from CRM & ERP and fed through Bronze → Silver → Gold

✔ Designed to support Power BI reporting and business decision-making

✔ Includes documentation, scripts, datasets, and test cases

📈 Future Enhancements

Add incremental load logic

Automate pipelines (e.g., Airflow, ADF)

Implement business-ready models in Gold

Integrate data quality rules

👤 Author
Mohamed assem  

Data Architect & BI Developer

📫 assemmohamed331@gmail.com  
