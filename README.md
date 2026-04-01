# AdTech Clickstream Analytics & Fraud Detection

This project simulates a real-world mobile advertising analytics workflow using a large-scale synthetic dataset.  
The goal is to analyze advertising traffic, detect suspicious patterns, and evaluate campaign performance using data analytics techniques.

Due to privacy and business restrictions, real advertising datasets are rarely publicly available. Therefore, this dataset was generated to mimic realistic AdTech data structures used by advertising technology platforms.

---

# Project Objectives

- Simulate a realistic advertising clickstream dataset
- Perform data cleaning and preprocessing
- Identify suspicious traffic patterns and potential fraud
- Analyze campaign performance and conversion metrics
- Practice relational data analysis using multiple tables

---

# Dataset Description

The dataset consists of three relational tables representing a typical advertising analytics pipeline.

### 1. Clicks Table
Contains click-level advertising traffic data.

Columns include:
- click_id
- campaign_id
- publisher_id
- user_id
- device_type
- country
- ip_address
- timestamp
- cost

### 2. Installs Table
Records app installations associated with user clicks.

Columns:
- install_id
- click_id
- install_timestamp

### 3. Revenue Table
Tracks post-install user revenue events.

Columns:
- user_id
- revenue
- event_timestamp

---

# Realistic Data Simulation

To better represent real-world production data, several characteristics were intentionally introduced:

- Fraud-like traffic patterns (bot clicks, click bursts)
- Suspicious publisher activity
- Missing values
- Inconsistent formatting
- Duplicate records
- Outlier values

These features allow the project to simulate common challenges faced by data analysts working with advertising data.

---

# Dataset Size

Approximate dataset scale used for analysis:

- Clicks: ~5,000,000 rows
- Installs: ~250,000 rows
- Revenue: ~100,000 rows

Due to GitHub file size limits, only a **sample dataset** is included in this repository.

---

# Project Workflow

The analytics pipeline followed in this project:

Raw Data
↓
Data Cleaning
↓
Exploratory Data Analysis (EDA)
↓
Fraud Detection
↓
Campaign Performance Analysis

---

# Key Analysis Areas

The project focuses on identifying:

- Suspicious IP addresses generating abnormal click volumes
- Click burst patterns indicating bot activity
- Publishers with unusually low conversion rates
- Campaign performance metrics such as install rate and revenue contribution

---

# Tools & Technologies

- Python
- Pandas
- NumPy
- Jupyter Notebook
- SQL (for relational analysis)
- Data Visualization tools (Power BI / Matplotlib / Seaborn)

---

# Repository Structure

## Repository Structure

```
adtech-fraud-detection-analysis
│
├── data
│   └── clicks_sample.csv
│
├── notebooks
│   ├── 01_data_generation.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_fraud_detection.ipynb
│   └── 04_campaign_analysis.ipynb
│
├── sql
│   └── analysis_queries.sql
│
├── dashboard
│   └── dashboard_mockup.png
│
├── images
│   └── project_pipeline.png
│
├── requirements.txt
│
└── README.md
```

---

# Learning Outcomes

Through this project, the following skills were practiced:

- Large-scale data simulation
- Data cleaning and preprocessing
- Fraud detection techniques
- Relational data analysis
- Analytical problem solving in AdTech environments

---

# Future Improvements

- Build an interactive dashboard for campaign analytics
- Implement machine learning models for fraud detection
- Perform deeper cohort and retention analysis

---

# Author

Sagar Kumar  
Data Analytics & Data Science Enthusiast
