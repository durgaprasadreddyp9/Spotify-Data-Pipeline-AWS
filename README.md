# 🎵 AWS Spotify Data Pipeline

## 📌 Overview
This project implements a **serverless, event-driven ETL data pipeline** using **AWS services** to efficiently process, query, and visualize **Spotify data**. The architecture leverages **AWS Glue, S3, Athena, and QuickSight** to ensure a **scalable and cost-effective data workflow**.

### 🔹 Key Features:
✅ **Serverless & Event-Driven** – No need for manual intervention.  
✅ **Automated Data Processing** – AWS Glue handles transformations.  
✅ **Schema Detection & Query Optimization** – AWS Glue Crawlers + Athena.  
✅ **Interactive Dashboards** – Insights via Amazon QuickSight.  

---


| AWS Service           | Purpose |
|-----------------------|---------|
| **S3 (Data Storage)** | Stores raw (staging) and transformed (data warehouse) data. |
| **AWS Glue (ETL)** | Extracts, transforms, and loads data for analysis. |
| **AWS Glue Crawler** | Automatically detects schema and updates the AWS Glue Data Catalog. |
| **Amazon Athena (SQL Querying)** | Runs SQL queries directly on S3 data. |
| **Amazon QuickSight (Visualization)** | Generates dashboards for insights. |

---

## 🚀 Implementation Steps

### 1️⃣ **IAM User Setup**
🔐 **Security First**: Created an IAM user following the **Principle of Least Privilege** to restrict unnecessary access.

### 2️⃣ **S3 Bucket Creation**
Structured as:
📂 **staging/** → Stores raw Spotify data.  
📂 **data_warehouse/** → Stores transformed, query-ready data.

### 3️⃣ **AWS Glue ETL Pipeline**
- Developed an **ETL job** in **AWS Glue Studio**.
- Applied **data transformations** with minimal coding.
- Saved transformed data to `data_warehouse/` in **Parquet format** for performance optimization.

### 4️⃣ **AWS Glue Crawler & Data Catalog**
- Configured an **AWS Glue Crawler** to detect schemas.
- Automatically updated the **Glue Data Catalog**, making data **query-ready for Athena**.

### 5️⃣ **Querying with Amazon Athena**
- Used **SQL queries** to analyze transformed Spotify data.
- No infrastructure setup required—Athena queries directly from **S3**.

### 6️⃣ **Data Visualization with Amazon QuickSight**
- Connected QuickSight to **Athena tables**.
- Built **interactive dashboards** showcasing:
  - 🎵 **Top Songs & Artists**
  - 📊 **Streaming Trends Over Time**
  - 🔄 **Genre Popularity Analysis**

---


