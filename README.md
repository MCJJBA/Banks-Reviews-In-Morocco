# Bank Reviews in Morocco Analysis

End-to-end ETL pipeline for analyzing customer reviews of Moroccan bank agencies using Google Maps data and machine learning–based sentiment analysis.

---

## 🎯 Project Overview

This project aims to analyze customer sentiment toward Moroccan banks by processing Google Maps reviews through a fully automated ETL pipeline.  

---

## ✨ Key Features

- 🤖 Automated Google Maps reviews extraction  
- 🌍 Multilingual sentiment analysis using machine learning models  
- 📊 Interactive dashboards and visual analytics  
- 🗃️ PostgreSQL-based data storage  
- 🔄 ETL orchestration using Apache Airflow  

---

## 🚀 Quick Start
```bash
# Clone the repository
git clone https://github.com/MCJJBA/Bank-Reviews-Morocco.git
cd Bank-Reviews-Morocco

# Create a virtual environment
python -m venv env
source env/bin/activate  # On Windows use: env\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## 🚀 Installation & Setup

### Prerequisites
- Python 3.7+
- pip package manager

### Installation Steps

1. **Install Apache Airflow**
```bash
   pip install apache-airflow
```

2. **Initialize Airflow**
   
   Run the following command to initialize the Airflow metadata database:
```bash
   airflow db init
```

3. **Set Up DAGs Folder**
   - Create a new folder named `airflow` at your desired location
   - Inside `airflow`, create another folder named `dags` (lowercase recommended)
   - Copy the contents of your repository's `airflow` folder into the newly created `airflow/dags` folder
   - Your Airflow DAGs should now be in: `airflow/dags/`

4. **Configure Airflow**
   
   (Optional) Point Airflow to your new DAGs folder by setting the `dags_folder` variable in `airflow.cfg` or via environment variable:
```bash
   export AIRFLOW__CORE__DAGS_FOLDER=$(pwd)/airflow/dags
```

5. **Start Airflow**
   
   Start the Airflow webserver and scheduler in separate terminals:
```bash
   # Terminal 1
   airflow webserver
   
   # Terminal 2
   airflow scheduler
```
   
   Access the Airflow UI at [http://localhost:8080](http://localhost:8080)

## 📊 Visualizations & Dashboard

### Dashboard Overview

The interactive dashboard provides comprehensive analytical insights through:

- Real-time sentiment analysis of customer reviews
- Comparative evaluation of bank performance
- Geographic distribution of customer feedback across regions
- Analysis of customer satisfaction and service quality trends
- Topic-based insights segmented by bank and region
- Monitoring of review volume and user activity patterns
- Visualization of sentiment distribution by bank
- Geographic satisfaction heatmaps
- Topic modeling results
- Time-series analysis of review trends
- Review volume by agency location
- Rating distribution charts

**View Dashboard:** [Looker Studio Dashboard](https://lookerstudio.google.com/u/0/reporting/c39b3ae9-5983-49ea-9340-c1c7adbf816b)

## 👤 Author

[@MouadChafiki](https://github.com/MCJJBA)


