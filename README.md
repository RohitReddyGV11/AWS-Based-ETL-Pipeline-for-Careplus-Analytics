# AWS-Based ETL Pipeline for Careplus Analytics


## 📌 Project Overview

This repository contains a **serverless ETL (Extract-Transform-Load) data pipeline** built on AWS that automates the ingestion, transformation, and warehousing of Careplus support logs and ticket data. The pipeline uses AWS services to store raw data in **Amazon S3**, transform it via **AWS Lambda** and **Glue**, and load the processed results into a **Redshift** data warehouse for analytics and reporting.

Once processed, the data is **visualized using Power BI** to derive actionable insights and support business reporting needs.

---

## 🧠 Architecture

The pipeline follows an event-driven, serverless design that enables scalable and cost-efficient data processing:

1. **Data Ingestion**  
   - Raw support logs and ticket datasets are stored in designated folders in an **S3 bucket**.

2. **Transformation Layer**  
   - AWS Lambda functions and AWS Glue jobs process and clean the data.  
   - Transformed files are stored in **Parquet format** (optimized for analytics).

3. **Data Warehousing**  
   - Transformed Parquet files are loaded to **Amazon Redshift**.  
   - SQL table schemas are defined using Redshift DDL scripts in the repository.

4. **Analytics & Visualization**  
   - SQL queries (via **Athena** or Redshift) are used for analysis.  
   - Power BI dashboard connects to Redshift for reporting.

📊 This architecture supports scalable ingestion with minimal management overhead and integrates smoothly with modern data analytics tools.

---

## 🔧 Tech Stack

- **Cloud Services**: AWS S3, AWS Lambda, AWS Glue, Amazon Redshift, Amazon Athena  
- **Data Formats**: CSV → Parquet  
- **Transformation**: Python scripts  
- **Analytics Tools**: Athena, Redshift SQL, Power BI  
- **Notebook Analysis**: Jupyter Notebook

---

## 🚀 Features

### ✅ Automated Data Ingestion  
Raw CSV datasets for support logs and tickets are automatically stored in S3 and made available for processing.

### ✅ Serverless ETL  
AWS Lambda functions trigger Glue jobs to perform data cleaning, transformation, and storage.

### ✅ Columnar Storage Optimization  
Transformed files are written as **Parquet**, enabling faster analytics and reduced processing costs.

### ✅ Scalable Data Warehouse  
Transformed data is loaded into **Amazon Redshift** for scalable analytics workloads.

### ✅ BI & Dashboards  
Integrated with **Power BI** to provide interactive business insights and visual reporting.

---

## 📊 Power BI Dashboard

A complete Power BI report — `Careplus-Insights.pbix` — is included to visualize pipeline results.  
You can **open the PBIX file** in Power BI Desktop and connect directly to your Redshift endpoint for live analytics.

🔗 *View Published Report [https://app.powerbi.com/view?r=eyJrIjoiMmU3MjlmZjktNzBmNy00OGJiLWE5N2MtYWQ3N2VkODNlMTQwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9]*
