Data Warehouse and Analytics Project

💡Project Overview
This project is a simple end-to-end ETL and data analytics project that I built while learning data engineering concepts through online tutorials and practice.

The main goal is to:

Load raw data from CSV files

Clean and transform the data using SQL

Build a structured data model for analysis

Run analytical queries to extract business insights

This project helped me understand how data flows from raw sources to analytics-ready tables.

🏗️ Architecture Overview

I followed a simplified Medallion Architecture, organized into three layers:

🥉 Bronze – Raw Data

Raw CSV files loaded into SQL Server

Data is stored as-is, without modifications

Purpose: keep a copy of the original data

🥈 Silver – Cleaned Data

Data cleaning and standardization

Handling missing values and inconsistent formats

Preparing data for analytics

🥇 Gold – Analytics Layer

Business-friendly tables

Fact and dimension tables (star schema)

Used for reporting and analysis

This layered approach makes the pipeline clear, scalable, and easy to debug.

⚙️ Tools & Technologies

SQL Server Express – Database engine

SQL Server Management Studio (SSMS) – SQL development & management

CSV Files – Source data

Draw.io – Architecture and data model diagrams

Git & GitHub – Version control

All tools used in this project are free.

🔄 ETL Process

Extract

Load CSV files into staging (Bronze) tables

Transform

Clean data (dates, nulls, duplicates)

Normalize column formats

Prepare keys for joins

Load

Insert clean data into Silver tables

Build analytics tables in the Gold layer

📊 Analytics & Reporting

Using the Gold layer, I created SQL queries to analyze:

Customer behavior

Product performance

Sales trends over time

These queries simulate real business questions and help practice analytical thinking with SQL.

📂 Project Structure

🎯 What I Learned

How ETL pipelines work in practice

How to structure a data warehouse

Difference between raw, cleaned, and analytics data

Writing cleaner and more efficient SQL
