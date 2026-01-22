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
source env/bin/activate

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
cp .env.example .env
# Update .env with your credentials

## ⚙️ Apache Airflow Setup & Initialization

Apache Airflow is used to orchestrate and automate the ETL workflows of this project. Follow the steps below to configure Airflow correctly.

### 1️⃣ Install Apache Airflow

It is highly recommended to install Airflow inside a Python virtual environment.

```bash
pip install apache-airflow
2. **Initialize Airflow**  
   - Run the following command to initialize the Airflow metadata database:
     ```bash
     airflow db init
     ```

3. **Set Up DAGs Folder**  
   - Create a new folder named `airflow` at your desired location.
   - Inside `airflow`, create another folder named `Dags` (case-sensitive).
   - Copy the contents of your repository’s `airflow` folder into the newly created `airflow/Dags` folder.
   - Your Airflow DAGs should now be in:  
     `airflow/Dags/`

4. **Configure Airflow**  
   - (Optional) Point Airflow to your new DAGs folder by setting the `dags_folder` variable in `airflow.cfg` or via the environment variable:
     ```bash
     export AIRFLOW__CORE__DAGS_FOLDER=$(pwd)/airflow/Dags
     ```

5. **Start Airflow**  
   - Start the Airflow webserver and scheduler in separate terminals:
     ```bash
     airflow webserver
     airflow scheduler
     ```
   - Access the Airflow UI at [http://localhost:8080](http://localhost:8080).

## 📊 Visualizations & Dashboard
### 📊 Dashboard Overview

The interactive dashboard provides comprehensive analytical insights through:
- real-time sentiment analysis of customer reviews,
- comparative evaluation of bank performance,
- geographic distribution of customer feedback across regions,
- analysis of customer satisfaction and service quality trends,
- topic-based insights segmented by bank and region,
- monitoring of review volume and user activity patterns,
- visualization of sentiment distribution by bank,
- geographic satisfaction heatmaps,
- topic modeling results,
- time-series analysis of review trends,
- review volume by agency location,
- and rating distribution charts.
My Dashboard : (https://lookerstudio.google.com/u/0/reporting/c39b3ae9-5983-49ea-9340-c1c7adbf816b)

# AUTHOR
[@MouadChafiki](https://github.com/MCJJBA)


