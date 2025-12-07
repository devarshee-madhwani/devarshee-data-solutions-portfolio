                ┌─────────────────────────┐
                │   Streaming Sources     │
                │  (POS, eComm, Sensors)  │
                └─────────────┬───────────┘
                              │ (JSON, Events)
                       ┌──────▼───────┐
                       │ Kafka / EH   │
                       │ (Event Hub)  │
                       └──────┬───────┘
                              │ Stream Processing
                      ┌───────▼────────┐
                      │ Stream Analytics│
                      │ / Spark Stream  │
                      └───────┬────────┘
                              │ (Processed Events)
        ┌─────────────────────▼─────────────────────┐
        │              Bronze Layer                 │
        │       (Raw Delta Lake Storage)            │
        └─────────────────────┬─────────────────────┘
                              │ Clean / Transform
        ┌─────────────────────▼───────────────────────┐
        │                Silver Layer                  │
        │     (Validated, Enriched Delta Tables)       │
        └─────────────────────┬────────────────────────┘
                              │ Modeling (dbt + PySpark)
        ┌─────────────────────▼────────────────────────────┐
        │                     Gold Layer                   │
        │   (Dimensional Models: Sales, Customer, SKU)     │
        └──────────┬───────────────┬───────────────┬──────┘
                   │               │               │
         ┌─────────▼──┐   ┌────────▼─────┐   ┌─────▼────────┐
         │ Power BI   │   │ AI/ML Models │   │ RAG Assistant │
         │ Dashboards │   │ Forecasting   │   │ (GPT + Vector)│
         └────────────┘   └──────────────┘   └───────────────┘

                       ┌─────────────────────────┐
                       │       Airflow DAG       │
                       │ Orchestrates All Steps  │
                       └─────────────────────────┘

