AWS Spotify Data Pipeline

This is a serverless, event-driven ETL data pipeline built using AWS services to process, query, and visualize Spotify data.

Architecture Overview:

S3 (Data Storage) – Stores raw (staging) and transformed (data warehouse) data.

AWS Glue (ETL) – Processes and transforms data for analysis.

AWS Glue Crawler – Automatically detects schema and updates the AWS Glue Data Catalog.

Amazon Athena (SQL Querying) – Queries structured data from S3 without moving it.

Amazon QuickSight (Visualization) – Creates dashboards and insights.

Implementation Steps:

1. IAM User Setup
Created an IAM user with the Principle of Least Privilege for security.

2. S3 Bucket Creation
Structured as:
staging/ → Raw data
data_warehouse/ → Transformed data

3. AWS Glue ETL Pipeline
Used AWS Glue Studio to create an ETL job for data transformation with minimal coding.

4. AWS Glue Crawler & Data Catalog
Configured a crawler to detect schemas, making data query-ready for Athena.

5. Querying with Amazon Athena
Queried transformed data using SQL without infrastructure setup.

6. Data Visualization with QuickSight
Built interactive dashboards for insights.
