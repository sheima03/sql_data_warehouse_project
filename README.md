# Data Warehouse & Analytics Project

![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![SSMS](https://img.shields.io/badge/SSMS-DA1F26?style=for-the-badge&logo=microsoft&logoColor=white)

## 💡 Project Overview
This project is an end-to-end **ETL (Extract, Transform, Load)** and data analytics pipeline. By moving data from raw CSV files into a structured SQL Server environment, this project simulates a real-world data warehousing workflow.

**The main objectives are:**
* **Ingest** raw data from flat files.
* **Clean and Transform** data using SQL.
* **Model** data for optimized querying.
* **Analyze** business performance.

---

## 🏗️ Architecture Overview
I implemented a **Medallion Architecture**, which organizes data into three distinct layers to ensure quality and traceability.



[Image of Medallion Architecture]


### 🥉 Bronze (Raw Layer)
* **Source:** Raw CSV files.
* **Storage:** Data is loaded "as-is" to keep a copy of the original records.

### 🥈 Silver (Cleaned Layer)
* **Process:** Data cleaning, deduplication, and standardization.
* **Tasks:** Handling nulls and correcting data types.

### 🥇 Gold (Analytics Layer)
* **Model:** Structured into **Fact and Dimension tables** (Star Schema).
* **Purpose:** Business-friendly tables used for reporting.



---

## ⚙️ Tools & Technologies
* **SQL Server Express:** Database engine.
* **SSMS:** SQL development and management.
* **Draw.io:** Architecture and data model diagrams.
* **Git & GitHub:** Version control.

---

## 🔄 ETL Process

1. **Extract:** Loading CSV data into **Bronze** staging tables.
2. **Transform:** Using SQL for type casting, removing duplicates, and normalizing formats.
3. **Load:** Populating the **Gold** layer with clean, analytical tables.

---

## 📂 Project Structure
```text
├── sql_scripts/
│   ├── 01_bronze_layer.sql
│   ├── 02_silver_layer.sql
│   ├── 03_gold_layer.sql
│   └── 04_analytics.sql
├── data/
│   └── raw_csv_files/
└── README.md
