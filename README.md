# 🌍 International Education Cost Analysis - ETL Pipeline

This project is a data engineering solution designed to help students, educators, and policymakers gain deeper insights into the cost of pursuing higher education internationally. It automates the ingestion, transformation, and aggregation of raw cost data using modern tools like Apache Airflow, Apache Spark, and Docker.

---

## 🧰 Tech Stack

- **Apache Airflow** – Workflow orchestration
- **Apache Spark (PySpark)** – Data transformation
- **Docker + Docker Compose** – Containerization
- **Pandas** - For Data Exploration
- **Matplot.lib** - For Exploratory Data Analysis

---
## 🚀 Setup & Execution Guide

### 📦 Prerequisites
- [Docker](https://www.docker.com/products/docker-desktop)
- [Docker Compose](https://docs.docker.com/compose/)

### 🛠️ Project Structure
DE_final_project/
├── dags/

│ └── etl_pipeline.py # Airflow DAG

├── spark_jobs/

│ └── transform.py # PySpark job

├── docker/

│ └── Dockerfile # Custom Docker image for Spark

├── data/

│ ├── International_Education_Costs.csv # Raw input data

│ └── output/ # Directory for transformed outputs

├── docker-compose.yml # Orchestration file



### 🧪 Step-by-Step Execution

1. **Clone the Repository**
   cd DE_final_project

### Build & Launch the Containers
docker-compose up --build
   
### Access the Airflow UI

Navigate to:http://localhost:8081

Username: airflow

Password: airflow

### Trigger the DAG

Go to the Airflow web interface

Enable and trigger the DAG named education_cost_etl_pipeline

### Check the Output

After execution, processed CSV files will be saved in the data/output/ folder.

