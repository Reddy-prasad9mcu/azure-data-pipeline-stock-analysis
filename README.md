# End-to-End Azure Data Pipeline for Stock Market Analysis 📈☁️

## 🔍 Overview
This project demonstrates an end-to-end Azure Data Engineering pipeline to ingest, process, and visualize stock market data using cloud-native services.

## 🚀 Tech Stack
- Azure Data Factory (ADF)
- Azure Data Lake Storage Gen2 (ADLS)
- Azure Synapse Analytics
- Power BI
- Alpha Vantage API
- SQL, Python


## 📂 Data Flow
1. **Ingestion**: ADF fetches stock data (MSFT, AAPL, GOOGL, AMZN) via REST API (Alpha Vantage) → stored in ADLS (`bronze`)
2. **Transformation**: Synapse queries and processes JSON to Parquet → (`silver`)
3. **Aggregation**: Compute 7-day moving averages → (`gold`)
4. **Visualization**: Power BI connects to gold layer for trend analysis

## 📊 Output
- Cleaned stock data
- Computed moving averages
- Power BI dashboard with visual trends

## 📌 Key Learnings
- Cloud-native ELT architecture
- JSON data handling in Synapse SQL
- Parameterized pipelines in ADF
