Project Title: Consolidated Data Lakehouse Pipeline (FMCG Domain)

Overview
This project simulates a real-world data engineering scenario where a parent company (Cult) acquires a smaller startup (SportsBar). The goal is to build a unified Lakehouse architecture using Databricks (Free Edition) to consolidate data from both companies, enabling unified business analytics.

Business Problem
Cult operates on mature ERP systems, while SportsBar has fragmented data stored across spreadsheets, cloud drives, and various exports. Management requires a single dashboard to track aggregated performance metrics across both entities.

Tech Stack
Platform: Databricks (Free Edition)

Storage: Amazon S3 (Data Lake)

Languages: Python (PySpark), SQL

Architecture: Medallion Architecture (Bronze, Silver, Gold layers)

Analytics: Databricks SQL Dashboards and Genie (AI-assisted insights)

Orchestration: Databricks Jobs

Key Features of the Pipeline
Data Ingestion: Established a connection between Databricks and AWS S3 to ingest raw transaction data.

Medallion Architecture:

Bronze: Raw data storage.

Silver: Data cleaning, handling nulls/negatives, and standardization.

Gold: Final business-ready tables for dimensional modeling.

Incremental Loading: Implemented robust logic to handle daily updates, keeping the warehouse current without redundant processing.

Orchestration: Automated the entire workflow using Databricks Jobs for daily execution.

Unified Reporting: Built a BI dashboard and utilized Genie AI to query and visualize consolidated revenue and product performance across both companies.

Setup Instructions
Configure Databricks Free Edition workspace.

Set up AWS S3 buckets and credentials for storage.

Follow the notebook order provided in the repository to recreate the Bronze-to-Gold flow.
