# Data-Modeling-Project-with-Databricks-and-PySpark
Data modeling project using Databricks and PySpark for ETL processes, data transformation, and analysis.
This project focuses on data modeling utilizing PySpark SQL within the Databricks environment. The aim is to create a multi-layer architecture for processing and storing sales data, comprising Bronze, Silver, and Gold layers.

## Table of Contents
1. [Project Structure](#project-structure)
2. [Data Model](#data-model)
3. [Layers](#layers)
   - [Bronze Layer](#bronze-layer)
   - [Silver Layer](#silver-layer)
   - [Gold Layer](#gold-layer)

---

## Project Structure

## Data Model
The data model incorporates various dimensions and facts related to sales transactions:

- **DimCustomers**: Information about customers
- **DimProducts**: Details about products
- **DimPayments**: Types of payments
- **DimRegions**: Geographic regions
- **DimSales**: Detailed sales information
- **FactSales**: Fact table linking dimensions with transactional data

## Layers

### Bronze Layer
The Bronze layer contains raw data collected from various sources. The initial load of this data is performed through SQL statements in `source.ipynb`.

### Silver Layer
The Silver layer transforms the raw data into a more structured format that includes derived fields, such as uppercase customer names. This is achieved in `silver.ipynb` through SQL transformations and additional processing.

### Gold Layer
The Gold layer consists of dimensional modeling, creating separate dimension tables for customers, products, payment types, and regions. Fact tables are created to link these dimensions with transactional data. This is defined in `gold.ipynb`.





