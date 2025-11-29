# Sql-Data-Warehouse-Project
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

Business-driven layer (currently no direct loading).

Intended for dashboards, KPIs, curated views, and analytics models.

Supports Power BI and ad-hoc SQL analysis.

📊 Analytics & Consumption

Designed to support Power BI, self-service analytics, and ad hoc queries.

Allows business users and analysts to explore integrated CRM and ERP insights.

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
