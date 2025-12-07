# AI-Enabled Omnichannel Retail Intelligence Platform (Flagship Project)

## Overview
An end-to-end enterprise retail analytics platform integrating batch + streaming ingestion, medallion lakehouse architecture, predictive modeling, AI-driven insights, and BI visualization. Built using Microsoft Fabric, Databricks, Python, SQL, Kafka/Event Hub, dbt, and Airflow.

## Problem Statement
Retail leaders require unified insights across in-store and online channels, real-time monitoring, forecasting, and AI recommendations to optimize operations, pricing, and inventory—but data is scattered across systems.

## Architecture Components
1. **Streaming Ingestion**  
   - Kafka or Azure Event Hub  
   - Stream Analytics or Spark Structured Streaming  

2. **Lakehouse (Medallion Architecture)**  
   - Bronze (raw), Silver (cleaned), Gold (dim/fact)  
   - Delta Lake  

3. **Transformation Layer**  
   - dbt models  
   - PySpark notebooks  
   - Fabric Dataflows Gen2  

4. **ML & AI Layer**  
   - Demand Forecasting (Prophet, ARIMA, LightGBM)  
   - Recommender System (Collaborative Filtering)  
   - Anomaly Detection (Isolation Forest)  
   - GenAI Insights (GPT summaries)  
   - Optional RAG Product Q&A  

5. **Orchestration**  
   - Airflow DAGs  

6. **Consumption Layer**  
   - Power BI dashboards (sales, inventory, customer segments)  
   - Real-time dashboard  
   - AI narrative panel  

## Tools & Technologies
- Power BI  
- Microsoft Fabric  
- Databricks (PySpark, MLFlow)  
- Python (Pandas, Scikit-Learn, XGBoost, Prophet)  
- Kafka / Event Hub  
- dbt  
- SQL  
- Airflow  
- Docker (optional for deployment)  

## Key Steps
1. Build streaming pipeline for real-time retail events.  
2. Develop medallion lakehouse using Fabric + Databricks.  
3. Implement dbt transformations for Gold layer.  
4. Train forecasting and recommendation models.  
5. Implement AI assistant for insights.  
6. Build Power BI omnichannel dashboard.  
7. Orchestrate workflows using Airflow.  

## Folder Structure
- `/architecture` – diagrams  
- `/data_models` – dimensional models  
- `/lakehouse` – bronze/silver/gold scripts  
- `/streaming` – Kafka/Event Hub scripts  
- `/notebooks` – Python/Spark notebooks  
- `/sql` – modeling SQL  
- `/databricks` – notebook exports  
- `/airflow` – DAG scripts  
- `/ai_prompts` – prompts for GPT/RAG  
- `/images` – dashboard screenshots  

