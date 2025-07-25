# 🛒 SmartCart: Purchase Pattern Analytics & Customer Segmentation Pipeline

**SmartCart** is a production-grade retail analytics pipeline designed to help businesses extract insights from invoice-level data. This project enables customer segmentation, purchase behavior analysis, and KPI tracking using automated ETL workflows, machine learning models, and dynamic BI dashboards.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## 📋 Table of Contents
- [Business Problem](#business-problem)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Data Source & Ethics](#data-source--ethical-considerations)
- [Tech Stack](#tech-stack)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Business Problem

Retail and e-commerce companies often struggle to:
- Identify high-value vs. churn-prone customers
- Forecast product demand with accuracy
- Track real-time sales and operational KPIs across categories
- Automate insights without manual intervention

**SmartCart** addresses these challenges through a scalable analytics solution.

## 📁 Project Structure

```
Smartcart_Retail_Analytics/
│
├── notebooks/                     # Jupyter notebooks for analysis and development
│   ├── ecomm_eda.ipynb           # Main exploratory data analysis notebook
│   └── model_dev.ipynb           # Model development and evaluation notebook
│
├── src/                           # Source code for the project
│   ├── dags/                     # Airflow DAGs for ETL workflows
│   │   └── transform_load.py     # Data transformation and loading logic
│   └── config/                   # Configuration files
│
├── terraform/                     # Infrastructure as Code (IaC) for GCP
│   └── gcp/                      # GCP-specific configurations
│       └── main.tf               # Main Terraform configuration
│
├── data/                          # Data storage (not versioned)
│   └── ecomm_invoice_transaction.parquet  # Processed data file
│
├── lib/                           # External dependencies
│   └── gcs-connector-3.0.7-shaded.jar  # Google Cloud Storage connector for Spark
│
├── sandbox/                       # Experimental code and tests
│   └── pyspark_transformation_test.ipynb  # PySpark experimentation
│
├── tests/                         # Test files
├── docs/                          # Project documentation
├── web-scraping/                  # Web scraping utilities and scripts
├── docker/                        # Docker container configurations
└── credentials/                   # Store for credential files (in .gitignore)
```

### Key Files and Their Purposes

#### Core Analysis Files
- `notebooks/ecomm_eda.ipynb`: Main notebook for exploratory data analysis
- `notebooks/model_dev.ipynb`: Notebook for model development and evaluation
- `sandbox/pyspark_transformation_test.ipynb`: Experimental PySpark code and tests

#### Data Pipeline
- `src/dags/transform_load.py`: ETL pipeline for data transformation and loading
- `src/config/`: Configuration files for the data pipeline

#### Infrastructure
- `terraform/gcp/main.tf`: GCP infrastructure configuration using Terraform
- `docker/`: Docker container configurations for deployment

#### Data
- `data/ecomm_invoice_transaction.parquet`: Processed dataset used for analysis

#### Dependencies
- `requirements.txt`: Python package dependencies
- `pyproject.toml`: Python project configuration (for Poetry)
- `poetry.lock`: Lock file for Poetry dependency management

#### Configuration
- `.gitignore`: Specifies intentionally untracked files to ignore
- `.pre-commit-config.yaml`: Pre-commit hooks configuration
- `ruff.toml`: Configuration for the Ruff linter

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Required Python packages (see `requirements.txt`)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/smartcart-retail-analytics.git
   cd smartcart-retail-analytics
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Analysis
1. Launch Jupyter Notebook:
   ```bash
   jupyter notebook analysis/notebooks/
   ```
2. Open `01_eda.ipynb` to start with exploratory data analysis

## 🔍 Data Source & Ethical Considerations

This project uses anonymized e-commerce transaction data for educational and demonstration purposes. Key points to note:

- **Data Anonymization**: All personally identifiable information has been removed
- **Ethical Web Scraping**: Data collection follows ethical guidelines including:
  - Respect for robots.txt rules
  - Rate-limited requests
  - No collection of personal or sensitive information
- **Purpose**: Strictly for educational and portfolio demonstration
- **Attribution**: Proper attribution given to data sources in compliance with terms of use

For detailed scraping methodology and ethical considerations, see the [web-scraping/README.md](web-scraping/README.md)

## 🛠 Tech Stack

| Layer            | Tools                            |
|------------------|----------------------------------|
| **Programming**  | Python, SQL                      |
| **Data Processing** | Pandas, NumPy, PySpark         |
| **BI Dashboards**| Power BI, Tableau                |
| **Data Modeling**| Scikit-learn, Statsmodels        |
| **Automation**   | Airflow, Docker                  |
| **Cloud**        | GCP, AWS                         |
| **Version Control** | Git, GitHub                    |

## 🤝 Contributing

Contributions are welcome! Please read our [contributing guidelines](CONTRIBUTING.md) before submitting pull requests.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


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


---

## Project Status

- ✅ Invoice data analysis, segmentation, dashboarding – **Complete**
- 🛠️ MLOps components (Airflow, Docker) – Implemented pipeline structure; refining for production-readiness
- ☁️ Cloud deployment (GCP, AWS) – Repository structured for cloud; deployment steps to be documented

---

## How to Use
1. Clone the repo

2. Install dependencies:
```text
pip install -r requirements.txt
```
3. Explore EDA and modeling in the notebooks/ directory

4. Open ecomm_bi.pptx to view Power BI dashboard

5. Dashboard automation via Airflow → coming soon

