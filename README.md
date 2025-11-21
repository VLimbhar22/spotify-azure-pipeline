# 🎧 Spotify Data Engineering Pipeline on Azure

## 📘 Project Overview
This project demonstrates an end-to-end data engineering pipeline built on **Microsoft Azure** using **Spotify streaming data**.  
It automates data ingestion, transformation, and analytics leveraging Azure cloud services and modern data engineering practices.

---

## ⚙️ Architecture

**Data Flow:**
1. **Data Ingestion:** Spotify API → Azure Data Lake Storage Gen2 (Bronze layer)
2. **Data Processing:** Azure Databricks (Silver layer) using PySpark for cleaning and transformation
3. **Data Curation:** Delta Lake tables (Gold layer) ready for analytics
4. **Orchestration:** Azure Data Factory (ADF) pipelines and triggers
5. **Analytics & Visualization:** Power BI / Synapse for reporting

**Architecture Diagram:**


---

## 🧩 Tech Stack

| Category | Tools / Services |
|-----------|------------------|
| Cloud Platform | Azure |
| Storage | Azure Data Lake Gen2 |
| Processing | Azure Databricks (PySpark) |
| Orchestration | Azure Data Factory |
| Data Format | Parquet / Delta |
| Visualization | Power BI |
| Source | Spotify Web API |

---

## 🛠️ Key Features
- Automated ETL pipeline with ADF and Databricks notebooks  
- Incremental data ingestion using event triggers  
- Delta Live Tables with SCD Type-2 support  
- Medallion architecture (Bronze → Silver → Gold)  
- Optimized PySpark transformations for better performance  
- Reusable modular notebooks and parameterized pipelines

---

## 📂 Project Structure
```bash
spotify-azure-pipeline/
│
├── notebooks/              # Databricks notebooks for ETL & transformations
├── adf_pipelines/          # JSON definitions for Azure Data Factory
├── configs/                # Connection strings, credentials (excluded in .gitignore)
├── resources/              # Architecture diagrams, documentation
└── README.md               # Project documentation

