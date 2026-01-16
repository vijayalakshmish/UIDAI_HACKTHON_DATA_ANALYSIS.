# UIDAI_HACKTHON_DATA_ANALYSIS.
# 🏆 UIDAI Data Hackathon 2026  
## Unlocking Societal Trends in Aadhaar Enrolment & Demographics

---

## 📌 Project Overview

This project presents an end-to-end, policy-oriented analytical framework built on **UIDAI Aadhaar Enrolment and Demographic datasets**.  
The objective is to uncover **meaningful societal patterns, regional disparities, temporal trends, anomalies, and predictive signals** that can support:

- Evidence-based government decision-making  
- Infrastructure and enrolment center planning  
- Inclusion and accessibility improvements  
- Continuous monitoring of Aadhaar system performance  

The solution combines **rigorous data preprocessing, advanced exploratory analysis, anomaly detection, forecasting, and interactive dashboards**, making it suitable for **national-scale governance analytics**.

---

## 🎯 Problem Statement

Despite widespread Aadhaar adoption, enrolment patterns vary significantly across regions, age groups, and time periods.  
These variations are often hidden within large-scale datasets and are difficult to translate into actionable insights.

**This project addresses:**
- Where enrolment gaps persist
- Which demographic segments are underrepresented
- How enrolment trends evolve over time
- How anomalies and future demand can be detected early

---

## 📂 Datasets Used (UIDAI Official)

### Demographic Data
- `api_data_aadhar_demographic_0_500000.csv`
- `api_data_aadhar_demographic_500000_1000000.csv`
- `api_data_aadhar_demographic_1000000_1500000.csv`
- `api_data_aadhar_demographic_1500000_2000000.csv`
- `api_data_aadhar_demographic_2000000_2071700.csv`

### Enrolment Data
- `api_data_aadhar_enrolment_0_500000.csv`
- `api_data_aadhar_enrolment_500000_1000000.csv`
- `api_data_aadhar_enrolment_1000000_1006029.csv`

> 📌 All datasets are sourced exclusively from UIDAI / data.gov.in as per hackathon rules.

---

## 🧹 Data Preprocessing & Engineering

### Key Steps
- Merged multi-part CSVs into unified datasets
- Removed duplicate records
- Handled missing values:
  - Dropped invalid Aadhaar IDs
  - Median imputation (age)
  - Mode imputation (gender)
  - Dropped unparseable dates (`NaT`)
- Standardized text fields (state, district)
- Outlier detection & treatment using IQR capping
- Temporal feature extraction (year, month, quarter)
- Age group aggregation & proportion calculations
- Dataset integration for multivariate analysis

### Saved Outputs
- `clean_demographics.csv`
- `clean_enrolment.csv`
- `clean_merged_aadhaar_data.csv`

---

## 📊 Analysis & Visualizations

### Univariate Analysis
- Age and demographic distributions
- State & district-wise enrolment volumes
- Yearly and monthly enrolment patterns

### Bivariate & Multivariate Analysis
- Age group vs enrolment patterns
- State × Age × Time relationships
- Correlation analysis
- Heatmaps for enrolment intensity

### Advanced Analytics
- **Anomaly detection** using statistical thresholds
- **Predictive trend forecasting** using Linear Regression
- PCA-ready feature engineering (optional extension)

### Visualization Types Used
- Histograms
- Bar charts
- Line plots
- Boxplots
- Heatmaps
- Scatter plots (anomaly detection)
- Forecast trend overlays

---

## 📈 Power BI Dashboard

An interactive Power BI dashboard was developed to operationalize insights for administrators.

### Dashboard Features
- State & district-level enrolment comparison
- Time-series enrolment monitoring
- Demographic segmentation
- Anomaly identification
- Policy-ready KPI views

📁 Power BI file (`.pbix`) available in this repository.

---

## 🧠 Key Insights & Impact

- Significant regional disparities exist despite high aggregate enrolment
- Age-based enrolment trends indicate future service demand
- Temporal anomalies highlight targeted enrolment drives or policy events
- Predictive trends support proactive infrastructure planning

---

## 🇮🇳 Policy Alignment

### Digital India
- Strengthens Aadhaar as digital public infrastructure
- Enables data-driven governance
- Supports last-mile inclusion initiatives



---

## ⚠️ Limitations

- Aggregated data limits pincode-level precision
- Static historical data (no real-time feeds)
- Limited demographic variables
- Correlation-based insights (not causal)

---

## 🔮 Future Scope

- Real-time enrolment monitoring (Microsoft Fabric pipelines)
- Advanced forecasting (ARIMA / LSTM)
- Inclusion gap scoring
- Policy impact simulation
- Fraud & anomaly risk modeling

---

## 🛠️ Tech Stack

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Power BI
- Microsoft Fabric (design compatibility)
- Google Colab

---




