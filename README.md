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

![Architecture Diagram]() 

## 🚀 Key Features
* **Ingestion:** Automated data extraction from the Ergast F1 API using Python/ADF.
* **Transformation:** * **Bronze:** Raw JSON ingestion.
    * **Silver:** Data cleaning, schema enforcement, and joining normalized tables (Drivers, Constructors, Results).
    * **Gold:** Business-level aggregations (e.g., `normalized_points`, `constructor_dominance`) ready for BI.
* **Visualization:** Interactive Power BI dashboard with 3 pages (Legends, Teams, Nations) featuring dynamic "Eras of Dominance" analysis.

## 📊 Dashboard Previews
### Page 1: Driver Legends
![Legends Dashboard]()

### Page 2: Constructor Wars
![Teams Dashboard]()

## 💻 How to Run
1.  Clone the repo.
2.  Mount Azure Storage in Databricks using the setup notebook.
3.  Run the Ingestion pipelines...
