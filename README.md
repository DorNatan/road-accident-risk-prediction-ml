# Road Risk Prediction using Machine Learning

## Overview
This project builds an end-to-end machine learning system designed to proactively identify high-risk road segments before accidents occur.

Using real-world data from intercity roads in Israel (2021–2024), the system integrates accident history, infrastructure features, traffic volume, and geospatial data into a unified dataset of ~40,000 road segments.

The goal is to support proactive decision-making in road safety and infrastructure planning.

---

## High-Risk Road Segments (Geospatial Analysis)

<img width="1107" height="715" alt="image" src="https://github.com/user-attachments/assets/0b384277-202e-448c-b693-e1d8da4453ab" />


The model identifies high-risk road segments and visualizes them using geospatial analysis, enabling clear detection of critical hotspots.

---

## Model Performance

<img width="798" height="704" alt="image" src="https://github.com/user-attachments/assets/dcc712de-0c64-499d-8835-9f1dc52f5476" />


The model demonstrates strong classification performance, with high recall (critical for safety applications) and balanced precision.

---

## Feature Importance

<img width="792" height="476" alt="image" src="https://github.com/user-attachments/assets/a3af4563-534e-4158-b891-fc2730bd1f65" />


Key features influencing risk include infrastructure conditions, traffic volume, and road geometry.

---

## Data Analysis (Correlation Heatmap)

<img width="944" height="999" alt="image" src="https://github.com/user-attachments/assets/108ea7a9-d415-4f65-9a73-61fd7815d50a" />


Exploratory analysis highlights relationships between variables and supports feature selection.

---

## Composite Risk Score

<img width="1237" height="587" alt="image" src="https://github.com/user-attachments/assets/6b69e975-54bf-4780-9aee-c79d4c33e54c" />


A custom Composite Risk Score (0–1) was developed to provide a continuous and interpretable ranking of road segment risk.

---

## Methodology

### Data Preparation
- Merged multiple datasets into unified road segments (500m resolution)
- Handled missing values using statistical and KNN-based methods
- Standardized and cleaned features

### Feature Engineering
- Speed-to-curvature ratio  
- Distance to safety barriers  
- Traffic volume per lane  
- Additional domain-specific features  

### Modeling
- Logistic Regression  
- Random Forest  
- XGBoost  
- Ensemble model using Voting Classifier  

### Clustering
- KMeans clustering to identify different types of risk patterns:
  - Infrastructure-related risk  
  - Traffic-related risk  

---

## Performance Metrics
- ROC-AUC: up to 0.91  
- Recall: up to 85%  
- F1-score: ~0.71–0.76  

---

## Business Impact
- Enables proactive identification of dangerous road segments  
- Supports prioritization of infrastructure investments  
- Helps reduce severe accidents and improve road safety  

---

## Technologies
- Python  
- Pandas, NumPy  
- Scikit-learn, XGBoost  
- Matplotlib, Seaborn  
- Geospatial analysis  
