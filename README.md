# DataBricksOperation

## Overview  
This repository demonstrates practical data operations performed using **Databricks**, including:
- Creating Delta tables from CSV data  
- Performing SQL-based data summarization  
- Building an interactive ETRM (Energy Trading and Risk Management) Dashboard  
- Setting up automated **email alerts** for abnormal price patterns using Python  

---

## Key Notebooks

### 1. `SQL_DeltaTablePractice.ipynb`
**Task:** Create a Delta table from an existing dataset using SQL.  
**Description:** Demonstrates how to use SQL to convert a standard table to Delta format and validate the conversion.

---

### 2. `CSV_Filter.ipynb`
**Task:** Filter filenames ending with `.csv` using Python list comprehension.  
**Description:** A simple example showing efficient file filtering logic for preprocessing data.

---

### 3. `etrm_data_processing.ipynb`
**Task:** Read energy trade data, clean column names, and store as Delta tables.  
**Description:**  
- Reads CSV files from Databricks volumes  
- Cleans invalid column names  
- Converts and saves to Delta format (`etrm_trades_table`, `energy_summary_table`, `daily_summary_table`)

---

### 4. `etrm_sql_queries.sql`
**Task:** SQL queries for dashboard creation.  
**Includes:**  
- Total revenue and quantity per energy type  
- Daily revenue and volume trends  
- Aggregated energy performance metrics  

These queries power the **ETRM Dashboard visualizations** in Databricks SQL.

---

### 5. `etrm_alerts.ipynb`
**Task:** Detect abnormal energy prices and send alert emails.  
**Features:**  
- Detects values outside predefined thresholds  
- Logs alerts into a Delta table (`etrm_alert_logs`)  
- Sends alert emails automatically using Gmail SMTP  

---

## Interactive Dashboard  
Explore the **live interactive ETRM Dashboard** built in Databricks:  
 [View Published Dashboard Here](https://dbc-51440d65-cd14.cloud.databricks.com/dashboardsv3/01f0b363d69f166cad9fddafff95e24d/published?o=2682693863009682)

**Dashboard Visualizations:**
- Daily Revenue Trend (Line Chart)  
- Revenue by Energy Type (Bar Chart)  
- Total Volume by Day (Area Chart)  
- Alerts for Abnormal Prices  

The dashboard refreshes automatically based on the latest Delta table data.

---

## 🗂 Repository Structure
DataBricksOperaion/
├── README.md
├── SQL_DeltaTablePractice.ipynb
├── CSV_Filter.ipynb
├── etrm_data_processing.ipynb
├── etrm_sql_queries.sql
├── etrm_alerts.ipynb

---

## How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/myimaginations/DataBricksOperaion.git

   Import the notebooks into your Databricks workspace.

Execute notebooks in order:
etrm_data_processing.ipynb
etrm_sql_queries.sql
etrm_alerts.ipynb
Open the Dashboard using the published link above or within your Databricks workspace.

Author
Preeti Sahani
Exploring Data Engineering and Automation through Databricks Free Edition

“Learning by building, automating, and visualizing data.”
