# SupplySight: Predictive Supply Chain Disruption Mitigation

## Introduction

SupplySight is a project aimed at developing a real-time, predictive dashboard to mitigate supply chain disruptions. By leveraging machine learning for anomaly detection and forecasting, SupplySight provides businesses with actionable insights to ensure operational continuity and customer satisfaction. This project focuses on simulating and analyzing IoT sensor data, sales, inventory, and external data sources to predict and visualize potential supply chain disruptions.

## Problem Statement & Business Value

Global supply chains are increasingly vulnerable to disruptions caused by various factors, including natural disasters, geopolitical events, and economic fluctuations. Businesses need to proactively identify these disruptions and mitigate their impact to ensure operational continuity and customer satisfaction.

SupplySight addresses this problem by:

* **Real-time Anomaly Detection:** Identifying unusual patterns in sensor data that may indicate potential disruptions.
* **Predictive Disruption Alerts:** Using machine learning to forecast demand and predict disruptions based on external factors.
* **Interactive Dashboard:** Visualizing key metrics and anomalies to enable users to make data-driven decisions.

The business value of SupplySight includes:

* **Reduced Operational Costs:** By preventing disruptions, businesses can minimize losses and avoid costly downtime.
* **Improved Customer Satisfaction:** Ensuring timely delivery and maintaining product availability enhances customer satisfaction.
* **Enhanced Decision-Making:** Providing real-time insights empowers businesses to make informed decisions and take proactive measures.
* **Competitive Advantage:** Gaining a competitive edge by anticipating and mitigating disruptions before they impact the business.

## Tech Stack

The SupplySight project utilizes the following technologies:

* **Python:** The primary programming language for data processing, machine learning, and dashboard development.
* **Pandas:** For data manipulation and analysis.
* **Scikit-learn:** For machine learning model development and evaluation.
* **MLflow:** For tracking machine learning experiments and managing models.
* **Streamlit:** For creating interactive dashboards.
* **Plotly Express:** For data visualization.
* **CSV:** For data storage during initial development.
* **GitHub:** For version control and collaboration.
* **GitHub Pages:** For hosting project documentation.
* **Databricks (Future):** For scalable data processing, machine learning, and deployment.

## Development Process

The development process of SupplySight is divided into the following phases:

* **Phase 1: Data Simulation and Anomaly Detection:**
    * Simulating IoT sensor data, sales, inventory, and external data sources.
    * Developing an anomaly detection model using machine learning.
    * Saving the results to CSV files.
* **Phase 2: MLflow Integration:**
    * Integrating MLflow for model tracking and experiment management.
    * Addressing issues with model logging and loading.
* **Phase 3: Local Dashboard Development:**
    * Creating an interactive dashboard using Streamlit to visualize key metrics and anomalies.
    * Enhancing the dashboard with advanced analytics and business insights.
* **Phase 4: Databricks Porting and Deployment (Future):**
    * Migrating all functionalities to Databricks.
    * Leveraging Databricks built-in capabilities for data processing, machine learning, and deployment.
    * Automating data pipelines and model retraining.
* **Documentation:**
    * Documenting the project using Markdown and hosting it on GitHub Pages.
 
## Problems and Resolutions

During the development process, we encountered and resolved the following issues:

* **`TensorSpec` Issue:**
    * Problem: Issues with saving and loading TensorFlow models using MLflow.
    * Resolution: Implemented a workaround by saving and loading the model's weights separately.
* **Pylance Warnings:**
    * Problem: Pylance reporting unresolved imports, even though the code was running correctly.
    * Resolution: Acknowledged that these were primarily static analysis warnings and focused on runtime functionality.
* **Data Structure:**
    * Problem: Ensuring that the data structure was correct between data generation, model input, and dashboard visualization.
    * Resolution: Added multiple tests, and refactored the code to be more modular.
* **Dashboard Data Loading:**
    * Problem: Ensuring that the correct data loading function was being called.
    * Resolution: Renamed functions, and ensured the correct file paths were being used.
* **Streamlit Duplicate Element Id:**
    * Problem: Multiple Streamlit checkboxes having the same id.
    * Resolution: added unique keys to each checkbox.
* **Moving Average Calculation:**
    * Problem: The moving average was calculating over the entire dataset, rather than a rolling window.
    * Resolution: The moving average calculation was adjusted to use the last 7 days of data.

## Areas for Improvement

The following areas have been identified for future improvement:

* **Real-time Data Processing:** Implementing a streaming data pipeline to process data in real-time.
* **Advanced Forecasting Models:** Exploring and implementing more advanced time-series forecasting models.
* **External Data Integration:** Integrating real-time external data sources, such as weather APIs and news feeds.
* **Databricks Deployment:** Porting the project to Databricks to leverage its scalable and enterprise-grade capabilities.
* **Enhanced Dashboard Interactivity:** Adding more interactive elements and visualizations to the dashboard.
* **Automated Alerting System:** Implementing a robust alerting system to notify users of potential disruptions.
* **Cost Optimization:** Optimizing the solution for cost-effectiveness.
* **Data Source Improvement:** Replacing simulated data with real world data from kaggle.
