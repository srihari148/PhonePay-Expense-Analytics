
# PhonePe Expense Analytics (Databricks)

## Overview
End-to-end expense analytics pipeline using Databricks medallion architecture.

## Architecture
Bronze → Silver → Gold

## Ingestion
PDF-based ingestion with archiving and idempotency.

## Processing
Incremental Silver processing with watermarks and DQ checks.

## Analytics
Gold aggregates powering Databricks SQL dashboards.

## Orchestration
Databricks Workflow with task dependencies.
