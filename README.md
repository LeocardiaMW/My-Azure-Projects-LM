# Azure Data Fundamentals Project

## Overview

This project was completed as part of the **Microsoft Azure Data Fundamentals (DP-900)** training course and demonstrates foundational knowledge of cloud computing, data storage, data processing, and analytics within the Microsoft Azure ecosystem. The project explored how different Azure services can be used to store, manage, ingest, and analyse data across relational, non-relational, and analytical workloads.

## Objectives

- Understand core cloud computing concepts and service models (IaaS, PaaS, and SaaS).
- Explore relational data solutions using **Azure SQL Database**.
- Work with non-relational data using **Azure Storage Accounts** and **Azure Cosmos DB**.
- Analyse large-scale datasets using **Microsoft Fabric Lakehouse**.
- Implement data ingestion and streaming solutions.
- Develop practical SQL skills for querying and analysing business data.
- Gain hands-on experience across multiple Azure data services and workloads. 【1-4e9095】

## Azure Services Used

### Azure SQL Database
Used to explore relational database concepts including:

- Creating and managing SQL databases
- Structuring tables and relationships
- Querying business data using SQL
- Performing data analysis and reporting

### Azure Storage Account
Used to store and manage unstructured and semi-structured data, including:

- Blob storage
- Files
- Data imports and exports
- Storage containers for analytics workloads

### Azure Cosmos DB
Used to understand non-relational (NoSQL) databases:

- JSON document storage
- Distributed database concepts
- Scalability and high availability
- Flexible schema design

### Microsoft Fabric Lakehouse
Used for analytical workloads and modern data analytics:

- Centralised storage for structured and unstructured data
- Data transformation and exploration
- Analytics across large business datasets
- Integration with reporting and business intelligence solutions

### Microsoft Fabric Eventstreams
Used to ingest real-time data into analytical environments:

- Streaming data collection
- Event-driven architecture concepts
- Real-time analytics pipelines
- Integration with Fabric analytics services

### Additional Ingestion Methods
Data was also ingested through:

- File uploads (CSV and structured datasets)
- Azure Storage integration
- Data pipelines and data movement processes
- Batch and streaming ingestion techniques

## SQL Skills Demonstrated

This project involved practical SQL querying and data analysis against sample retail and sales datasets.

### SELECT

Retrieve specific fields from datasets:

```sql
SELECT ProductName, SalesAmount
FROM Sales;
```

### WHERE

Filter records based on conditions:

```sql
SELECT *
FROM Sales
WHERE SalesAmount > 1000;
```

### ORDER BY

Sort data for reporting and analysis:

```sql
SELECT ProductName, SalesAmount
FROM Sales
ORDER BY SalesAmount DESC;
```

### GROUP BY

Aggregate business metrics:

```sql
SELECT Category, SUM(SalesAmount) AS TotalSales
FROM Sales
GROUP BY Category;
```

### JOINs

Combine related data from multiple tables:

```sql
SELECT c.CustomerName,
       o.OrderID,
       o.TotalAmount
FROM Customers c
JOIN Orders o
    ON c.CustomerID = o.CustomerID;
```

## Key Learning Outcomes

Through this project, I developed an understanding of:

- Cloud computing fundamentals and Azure architecture
- Differences between relational and non-relational databases
- Data storage strategies for structured, semi-structured, and unstructured data
- Data ingestion and movement across Azure services
- Real-time analytics using Eventstreams
- Analytical processing using Microsoft Fabric
- SQL querying techniques for business intelligence and reporting
- Data modelling, scalability, and cloud-based analytics solutions

## Example Business Scenario

Using retail and sales datasets, analysis was performed to:

- Identify top-selling products
- Calculate total revenue by category
- Analyse customer purchasing patterns
- Track sales performance over time
- Produce aggregated business insights for decision-making

These exercises demonstrated how Azure data services can work together to support modern data platforms, from ingestion and storage through to analytics and reporting.

## Skills Gained

- Microsoft Azure Fundamentals
- Azure SQL Database
- Azure Storage Account
- Azure Cosmos DB
- Microsoft Fabric Lakehouse
- Microsoft Fabric Eventstreams
- Data Ingestion and Integration
- Relational Data Modelling
- NoSQL Concepts
- SQL Query Development
- Data Analytics
- Business Intelligence Fundamentals
- Cloud Computing Concepts

## Conclusion

This DP-900 project provided hands-on experience with Microsoft's cloud data platform and demonstrated the ability to work across relational, non-relational, and analytical workloads. By combining Azure SQL Database, Azure Storage, Azure Cosmos DB, Microsoft Fabric Lakehouse, and Eventstreams, the project showcased key data engineering and analytics concepts while building practical skills in SQL-based data analysis and cloud-based data solutions.
