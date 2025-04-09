# 🚀 End-to-End Data Engineering Pipeline on Olympic Data

This project demonstrates a complete data engineering pipeline built using various Azure services. The goal is to ingest raw data related to Olympic Data from a public GitHub repository, process and transform it, and finally analyze it to gain meaningful insights.

![Architecture](https://github.com/user-attachments/assets/8dfd6393-d40e-45be-9cb4-7c1d1c3b0753)
--

## 🧰 Technologies Used

- **GitHub** – Source of raw data (CSV files)  
- **Azure Data Factory (ADF)** – Data ingestion using HTTP connector  
- **Azure Data Lake Storage Gen2 (ADLS Gen2)** – Data storage (raw + transformed)  
- **Azure Databricks** – Data transformation using PySpark  
- **Azure Synapse Analytics** – Data analysis and querying  

---

## 🔁 Pipeline Flow

1. **Data Ingestion**  
   - **Source:** Public GitHub repository  
   - **Tool:** Azure Data Factory  
   - **Method:** HTTP connector  
   - **Destination:** ADLS Gen2 (Raw Zone)

2. **Data Transformation**  
   - **Tool:** Azure Databricks (Notebook in PySpark)  
   - **Source:** Raw data from ADLS Gen2  
   - **Process:** Cleaning, filtering, and restructuring  
   - **Destination:** ADLS Gen2 (Transformed Zone)

3. **Data Analysis**  
   - **Tool:** Azure Synapse Analytics  
   - **Source:** Transformed data from ADLS Gen2  
   - **Purpose:** Generate insights using SQL queries
