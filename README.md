## Road Risk Prediction using Machine Learning

This project builds an end-to-end machine learning system designed to proactively identify high-risk road segments before accidents occur.

Using real-world data from intercity roads in Israel (2021–2024), the system combines accident records, infrastructure characteristics, traffic volume, and geospatial features into a unified dataset of ~40,000 road segments.

### Key Features
- Advanced feature engineering (speed-curvature ratio, traffic per lane, infrastructure metrics)
- Custom Composite Risk Score (0–1) for continuous risk ranking
- Ensemble model (Random Forest + XGBoost + Logistic Regression)
- KMeans clustering for identifying different risk patterns
- Geospatial analysis and visualization of risk hotspots

### Performance
- ROC-AUC: up to 0.91  
- Recall: up to 85% (critical for safety detection)  
- F1-score: ~0.7–0.76  

### Impact
Unlike traditional reactive analysis, this system enables proactive identification of dangerous road segments, supporting better prioritization of infrastructure investments and potentially saving lives.
