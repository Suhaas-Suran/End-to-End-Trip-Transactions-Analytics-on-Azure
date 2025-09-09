# End-to-End Trip Transactions Analytics on Azure

## 📌 Project Overview
This project builds an **end-to-end data engineering pipeline** to process and analyze **trip transaction and ride rating data** using **Azure Data Factory (ADF)**, **Azure Databricks**, and **Azure Data Lake Storage (ADLS Gen2)**.  
The pipeline is designed using the **Medallion Architecture (Bronze → Silver → Gold)** to ensure scalable ingestion, transformation, and analytics.

Key highlights:
- Automated ingestion of trip transactions from **Azure SQL Database** into ADLS.
- **Data transformation and cleaning** with PySpark in Databricks.
- **Delta Lake** used for ACID transactions, schema enforcement, and time travel queries.
- **Pipeline orchestration** and scheduling in ADF.
- **Pipeline resiliency** with Logic Apps for email alerts on execution status.

---

## 🏗️ Architecture
<img width="802" height="509" alt="image" src="https://github.com/user-attachments/assets/3ec0d3d2-16c5-4141-aedc-925322b02ea2" />

1. **Bronze Layer** → Raw trip transactions and ratings ingested into ADLS.  
2. **Silver Layer** → Data cleaned, structured, and enriched in Databricks using PySpark.  
3. **Gold Layer** → Aggregated data for analytics (driver performance, trip efficiency, customer insights).  
4. **ADF Pipelines** → Manages orchestration and incremental loads.  
5. **Logic Apps** → Sends automated notifications on pipeline completion/failure.  

---

## ⚙️ Tech Stack
- **Languages**: Python, SQL, PySpark  
- **Services**: Azure Data Factory (ADF), Azure Databricks, Azure Blob Storage, Azure SQL Database, Logic Apps  
- **Storage Format**: Delta Lake (time travel, schema enforcement, ACID compliance)

---

## 🔑 Use Cases
- Analyze **trip efficiency** (distance, duration, delays).  
- Gain insights into **customer behavior and driver performance**.  
- Automate **alerts and notifications** for pipeline monitoring.  
- Deliver **analytics-ready data** for dashboards and reporting.  

---

## 🚀 Execution Flow
1. Ingest raw trip and rating data → Bronze Layer.  
2. Transform and clean data in Databricks → Silver Layer.  
3. Aggregate and store analytics-ready data → Gold Layer.  
4. Schedule pipelines via ADF.  
5. Trigger notifications via Logic Apps.  

---

## 📊 Outcome
- Delivered a **scalable Azure-based data pipeline** for trip transaction analytics.  
- Produced **business-ready Delta tables** supporting advanced analytics.  
- Automated **end-to-end orchestration and monitoring** with ADF + Logic Apps.  

---

## 📖 References
- [Delta Lake Documentation](https://delta.io/)  
- [Azure Data Factory](https://learn.microsoft.com/en-us/azure/data-factory/introduction)  
- [Azure Databricks](https://learn.microsoft.com/en-us/azure/databricks/)  

---
