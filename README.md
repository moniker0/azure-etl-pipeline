# azure-etl-pipeline

# Building an ETL Pipeline from Azure SQL to Azure Data Lake using Azure Data Factory

1️⃣ Overview:

- Objective: Automate data extraction from Azure SQL DB into Azure Data Lake Storage.
- Tools Used: Azure SQL, ADF, ADLS, Parquet/CSV.


2️⃣ Architecture Diagram:

<img width="270" alt="pipeline_architecture" src="https://github.com/user-attachments/assets/43367168-3206-406c-8720-4c751349a3e4" />



3️⃣ Implementation Steps:

- Created Azure SQL Database with multiple tables.
- Designed an ADF pipeline with a parameterized ForEach loop.
- Configured Linked Services & Datasets for dynamic table extraction.
- Loaded structured OLTP data into ADLS in Parquet format.


4️⃣ Challenges & Solutions:

- Authentication Issues: Used Managed Identity for ADF.
- Storage Access Denied: Fixed ADLS Firewall & IAM permissions.
- Missing Tables: Ensured parameterized dataset & dynamic file paths.
