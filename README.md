# Stock Market Kafka Real Time Data Engineering Project

## Project Overview
This project focuses on building a real-time stock market data pipeline using Apache Kafka, AWS services (S3, Athena, Glue), and Python. The goal is to ingest, process, and analyze stock market data in a scalable, fault-tolerant, and efficient manner.



## Architecture 
<img src="Architecture.jpg">

## Architecture
- Data Source: Live stock market feed (can be simulated or obtained from APIs like Alpha Vantage, Yahoo Finance).
- Data Ingestion: Kafka producers push stock price updates to Kafka topics in real-time.
- Streaming Processing: Kafka consumers read data and store it in an AWS S3 bucket.
-Data Transformation & Schema Management:
  - AWS Glue Crawler scans raw data and creates a schema in the Glue Data Catalog.
    Data is stored in Parquet format for optimized querying.
  - Querying & Analysis: AWS Athena is used to perform SQL queries on stock market data.
  - Visualization & Reporting: Data can be connected to BI tools (Tableau, Power BI, Looker) for real-time insights.
- Technology Stack
 - Programming Language: Python
 - Real-Time Streaming: Apache Kafka
 - Cloud Services: Amazon Web Services (AWS)
 - S3: Stores raw and processed stock market data.
 - Glue Crawler & Glue Catalog: Automates schema discovery and data transformation.
 - Athena: Enables SQL-based querying over large-scale data.
 - EC2: Hosts Kafka brokers, producers, and consumers.
## Dataset
You can use any stock market dataset or real-time APIs. Some options include:

Simulated Data: Generate random stock prices using Python.
Live API Data: Use Yahoo Finance, Alpha Vantage, or IEX Cloud APIs.


