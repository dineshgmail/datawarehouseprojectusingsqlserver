Project Overview

This project implements a Data Warehouse using the Inmon (Top-Down) Architecture. Data is extracted from multiple source systems, loaded into a staging layer, transformed into a centralized Enterprise Data Warehouse (EDW) in Third Normal Form (3NF), and finally published to Data Marts for reporting and analytics.

Architecture
Source Systems
      |
      v
 Staging Layer
      |
      v
Enterprise Data Warehouse (3NF)
      |
      v
   Data Marts
      |
      v
Reports & Dashboards
Architecture Components
1. Source Systems

The project ingests data from multiple operational systems such as:

Customer Data
Product Data
Booking Data
Transaction Data
2. Staging Layer

The staging layer is used for:

Landing raw data
Data validation
Data cleansing
Deduplication
Initial transformations
3. Enterprise Data Warehouse (EDW)

The EDW serves as the centralized repository for enterprise data.

Features:

Third Normal Form (3NF) design
Reduced data redundancy
Improved data consistency
Single source of truth
4. Data Marts

Business-specific Data Marts are created from the EDW for analytical reporting.

Examples:

Sales Mart
Customer Mart
Finance Mart

These marts are typically designed using dimensional modeling (Star Schema).

ETL Process
Extract data from source systems.
Load raw data into the staging layer.
Perform data cleansing and validation.
Transform and load data into the EDW (3NF).
Create Data Marts from the EDW.
Build reports and dashboards for business users.
Technologies Used
Azure Data Factory (ADF)
Azure SQL Database
Azure Data Lake Storage (ADLS)
SQL
Power BI
Project Structure
Project
│
├── Source Data
├── Staging Layer
├── EDW
├── Data Marts
├── ETL Pipelines
├── SQL Scripts
└── Documentation
Benefits of Inmon Architecture
Centralized enterprise data repository
High data quality and consistency
Reduced data redundancy
Supports multiple business domains
Scalable for enterprise reporting
Future Enhancements
Incremental data loading (CDC)
Automated pipeline monitoring
Data quality framework
Metadata-driven ETL process

Author: Dinesh
Architecture: Inmon (Top-Down Data Warehouse Model)
Purpose: Enterprise Reporting and Analytics
