# SupplySight
SupplySight is a project aimed at developing a real-time, predictive dashboard to mitigate supply chain disruptions.

# Data Pipeline
graph TD
    A[Data Sources: Simulated/Real-Time Streaming] --> B(Data Ingestion);
    B --> C(Data Cleaning & Preprocessing);
    C --> D{ML Algorithms: Anomaly Detection, Forecasting};
    D --> E[Model Training & Continuous Improvement];
    E --> F(Data Analysis & Metrics Calculation);
    F --> G[Dashboard: Visualization & Notifications];
    A --> H[Data Storage: S3/Delta Lake];
    H --> B
