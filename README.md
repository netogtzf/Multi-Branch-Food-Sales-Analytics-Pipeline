# Multi-Branch Food Sales Analytics Pipeline

## Overview

This project simulates a cloud-based analytics pipeline for multiple university food service branches using Snowflake SQL and Tableau. The goal was to centralize transactional sales data from different restaurant concepts into a unified analytics model for reporting, KPI tracking, and business analysis.

The project follows a layered data architecture approach commonly used in modern Data Engineering and Analytics workflows:

RAW → STAGING → ANALYTICS

---

## Business Objective

Create a centralized analytics environment capable of:

* Integrating multi-branch restaurant sales data
* Standardizing transactional records
* Supporting KPI tracking and operational analysis
* Preparing analytics-ready datasets for BI dashboards

---

## Tech Stack

* Snowflake
* SQL
* Tableau / Tableau Public
* Python (supporting workflow)
* GitHub

---

## Data Architecture

### RAW Layer

Original CSV datasets loaded directly into Snowflake without modification.

Examples:

* RAW_DAVILAS
* RAW_SUSHIGO
* RAW_BURRITOS
* RAW_TACOS

---

### STAGING Layer

Data transformation and standardization layer.

Transformations included:

* Timestamp conversion using TRY_TO_TIMESTAMP
* Column standardization
* Data cleaning
* Multi-source schema alignment

Examples:

* STG_DAVILAS
* STG_SUSHIGO
* STG_BURRITOS
* STG_TACOS

---

### ANALYTICS Layer

Centralized analytics-ready tables designed for BI consumption.

Main table:

* ALL_ORDERS

This layer consolidates all restaurant branches using SQL UNION ALL operations.

---

## Key Features

* Multi-branch data integration
* Cloud-based data warehouse architecture
* SQL-based ETL transformations
* KPI-ready analytical datasets
* Standardized transactional model
* Tableau-ready reporting structure

---

## Example KPIs

* Total Sales
* Orders per Branch
* Average Ticket
* Peak Hours
* Payment Method Distribution
* Delivery Time Metrics
* Top Selling Products

---

## Example SQL Operations

* TRY_TO_TIMESTAMP
* UNION ALL
* Aggregations
* KPI calculations
* Data standardization
* Layered schema transformations

---

## Project Workflow

CSV Files
↓
Snowflake RAW
↓
Snowflake STAGING
↓
Snowflake ANALYTICS
↓
Tableau Dashboard

---

## Future Improvements

* Automated ingestion using Snowflake Stages
* Snowflake Tasks & Streams
* AWS integration (S3, Glue, Athena)
* Real-time dashboard refresh
* Advanced product categorization
* Predictive sales forecasting

---

## Dashboard

The final dashboard focuses on:

* Executive KPI overview
* Operational performance
* Sales trends
* Product performance
* Multi-branch comparison

---

## Author

Ernesto Gutiérrez
