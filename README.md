# F1_DataEngineering_Project

# 🏎️ Formula 1 Data Lakehouse & Analytics

## 📖 Project Overview
This end-to-end data engineering project builds a comprehensive Data Lakehouse to analyze 74 years of Formula 1 racing history. The goal was to answer the question: *"Who is the true G.O.A.T.?"* by normalizing points across different scoring eras and visualizing team dominance.

## 🏗️ Architecture
**Tech Stack:**
* **Cloud:** Azure (Resource Groups, Storage Accounts)
* **Storage:** Azure Data Lake Gen2 (ADLS) - Implements Medallion Architecture (Bronze, Silver, Gold)
* **Processing:** Azure Databricks (PySpark)
* **Orchestration:** Azure Data Factory (ADF)
* **Visualization:** Power BI

## 🚀 Key Features
* **Ingestion:** Automated data extraction from the Ergast F1 API using Python/ADF.
* **Transformation:** * **Bronze:** Raw JSON ingestion.
    * **Silver:** Data cleaning, schema enforcement, and joining normalized tables (Drivers, Constructors, Results).
    * **Gold:** Business-level aggregations (e.g., `normalized_points`, `constructor_dominance`) ready for BI.
* **Visualization:** Interactive Power BI dashboard with 3 pages (Legends, Teams, Nations) featuring dynamic "Eras of Dominance" analysis.
## 📊 Dashboard Previews

### Page 1: Driver Legends 🏎️
*A cross-era comparison normalizing points to the modern 2024 scoring system.*
![Legends Dashboard](04_PowerBI/The_Legends.png)

### Page 2: Constructor Wars 🛠️
*Visualizing the rise and fall of F1 dynasties over 70 years.*
![Teams Dashboard](04_PowerBI/The_Machine.png)

### Page 3: Global Powerhouses 🌍
*Geospatial analysis of winning nations.*
![Nations Dashboard](04_PowerBI/Nations.png)
