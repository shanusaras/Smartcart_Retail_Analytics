# 🛒 SmartCart: Purchase Pattern Analytics & Customer Segmentation Pipeline

**SmartCart** is a production-grade retail analytics pipeline designed to help businesses extract insights from invoice-level data. This project enables customer segmentation, purchase behavior analysis, and KPI tracking using automated ETL workflows, machine learning models, and dynamic BI dashboards.

---

## Business Problem

Retail and e-commerce companies often struggle to:
- Identify high-value vs. churn-prone customers
- Forecast product demand with accuracy
- Track real-time sales and operational KPIs across categories
- Automate insights without manual intervention

**SmartCart** addresses these challenges through a scalable analytics solution.

---

## Project Objectives

- Segment customers using behavioral metrics like RFM (Recency, Frequency, Monetary)
- Forecast product demand and customer churn using predictive modeling
- Visualize key business KPIs through interactive Power BI/Tableau dashboards
- Automate data ingestion, transformation, and analytics workflows for scalability

---

## Tech Stack

| Layer            | Tools                            |
|------------------|----------------------------------|
| **Programming**  | Python, SQL                      |
| **BI Dashboards**| Power BI, Tableau                |
| **Data Modeling**| Scikit-learn, Statsmodels        |
| **Automation**   | Airflow (in progress), Docker (learning) |
| **Cloud Ready**  | GCP, AWS (planned)               |

---

## Key Features

- ✅ Customer Segmentation using RFM scoring and clustering
- ✅ Demand Forecasting using time series models
- ✅ Real-time Dashboards for Sales & Customer KPIs
- ✅ Automated ETL Pipelines for data ingestion and transformation
- ✅ Clean modular architecture ready for MLOps integration

---

## Folder Structure

```text
smartcart-retail-analytics/
├── code/                  # Data transformation scripts
├── notebooks/             # EDA, modeling, segmentation notebooks
├── data/                  # Raw & cleaned invoice datasets
├── docker/                # Docker configuration (in progress)
├── docs/                  # Supporting documentation
├── credentials/           # Placeholder for keys (not tracked)
├── src/                   # Python modules for models, pipelines
├── terraform/             # IaC for cloud infra (planned)
├── tests/                 # Unit tests (in progress)
├── web-scraping/          # Scraping scripts for dynamic data
├── ecomm_bi.pptx          # Power BI dashboard file
├── requirements.txt       # Python dependencies
└── README.md              # You’re here.

```

---

## Key Deliverables

- Designed the complete analytics pipeline from raw invoice data to automated customer segmentation and KPI dashboards  
- Developed predictive models and RFM-based segmentation logic for demand and retention optimization  
- Automated ETL and reporting workflows using Python and SQL; deployed visual insights via Power BI  
- Structured the codebase for future scaling with MLOps and cloud integration in mind


## Project Status
- Invoice data analysis, segmentation, dashboarding – Complete

- MLOps & automation (Airflow, Docker) – Learning in progress

- Cloud deployment (GCP, AWS) – Planned

## How to Use
1. Clone the repo

2. Install dependencies:
```text
pip install -r requirements.txt
```
3. Explore EDA and modeling in the notebooks/ directory

4. Open ecomm_bi.pptx to view Power BI dashboard

5. Dashboard automation via Airflow → coming soon

