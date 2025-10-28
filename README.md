Careplus Data Pipeline
Introduction
This project provides a serverless data pipeline for the Careplus System, automating the ingest, transformation, and analysis of support logs and tickets using AWS services. The processed data is made available for reporting and analytics through Power BI.

Folder Structure
text
├── data-ingestion/
│   ├── support-logs/
│   └── support-tickets/
├── data-transformation/
│   ├── automate_support_log_etl.ipynb
│   └── automate_support_tickets_etl.ipynb
├── data-warehousing/
│   ├── parquet_files_overview.ipynb
│   └── RedShift Table-creation-queries.txt
│   └── support-logs.xlsx
│   └── support-tickets.xlsx
├── data-analytics
│   ├── Athena-sql-queries.txt
│   └── ad-hoc analysis.txt
│   └── Careplus-Insights.pbix
├── pipeline-architecture.jpg
├── README.md


Power BI Report
View the published Power BI report here: https://app.powerbi.com/view?r=eyJrIjoiMmU3MjlmZjktNzBmNy00OGJiLWE5N2MtYWQ3N2VkODNlMTQwIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9