# PhonePe Expense Analytics – Databricks Medallion Project

## Overview
This project implements an end-to-end expense analytics pipeline using Databricks and Medallion Architecture (Bronze → Silver → Gold).
The pipeline ingests realtime PhonePay transaction statements data in PDF format, transforms and enriches transactional data incrementally, and exposes curated Gold-layer aggregates for Databricks SQL dashboards.

The solution is designed with production-grade principles including idempotency, incremental processing, data quality checks, and workflow orchestration.

## Architecture
<img width="578" height="1004" alt="image" src="https://github.com/user-attachments/assets/350e0e7d-99b1-4fab-8a40-c67d4c454336" />



## Technologies Used
1. Databricks (Community / SQL / Workflows)
2. Apache Spark (PySpark)
3. Delta Lake
4. Unity Catalog
5. Databricks SQL Dashboards
6. Git (version control)

## Key Design Decisions
1. Medallion architecture for scalability and clarity
2. Gold-only dashboards for performance
3. Watermark-based incremental processing
4. DDLs version-controlled in Git
5. Source data archived post-processing

## How to Run
1. Upload PDF files to input volume
2. Trigger Databricks Workflow
3. Validate Bronze → Silver → Gold tables
4. Open Databricks SQL dashboard

## Orchestration
Databricks Workflow with task dependencies.

## Author Notes
This project demonstrates production-level data engineering practices including ingestion, transformation, orchestration, and analytics within the Databricks ecosystem.
