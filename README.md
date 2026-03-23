# Air Quality Forecasting & Anomaly Detection

1. Project Title & Short Description
An end-to-end time-series machine learning pipeline for air quality data, including:
- Data cleaning
- Feature engineering
- Anomaly detection
- Forecasting future CO levels
- Evaluation and visualization

2. Problem Statement
## Problem Statement

Air pollution is a major environmental issue that affects public health.  
This project aims to:

1. Detect anomalies in air quality sensor data.
2. Forecast if CO (Carbon Monoxide) levels will exceed a threshold in the next hour.

The goal is to provide actionable insights and early warnings for air pollution events.

3. Dataset
## Dataset

- Source: [Air Quality UCI Dataset](https://archive.ics.uci.edu/ml/datasets/Air+Quality)
- Data contains hourly measurements from an air quality monitoring station in Italy.
- Features include sensor readings for gases (CO, NMHC, NOx, etc.), temperature, and humidity.
- CSV format with semicolon separator (`;`) and comma decimal (`,`).

4. Features / Methodology
## Features & Methodology

### Data Cleaning
- Replace invalid sensor readings (-200) with NaN
- Interpolate and forward/backward fill missing values
- Combine Date and Time columns into a datetime index

### Feature Engineering
- Time-based features: hour, day_of_week, month, is_weekend
- Lag features: previous CO readings
- Rolling statistics and differences

### Anomaly Detection
- Isolation Forest to detect anomalies in CO, temperature, and sensor readings
- Scaled features for improved detection

### Forecasting / Classification
- Random Forest Classifier for predicting CO threshold exceedance
- TimeSeriesSplit for cross-validation
- Hyperparameter tuning using GridSearchCV
- Scaled features to prevent leakage

### Evaluation
- Accuracy, ROC-AUC, Confusion Matrix, Classification Report
- Feature Importance plot
- ROC Curve visualization

5. Project Structure
## Project Structure

AirQualityForecasting/
├── data/                # Raw CSV dataset
├── notebook/            # Exploratory analysis and experiments
├── src/                 # Python scripts
│   ├── load_clean.py
│   ├── feature_engineering.py
│   ├── anomaly_detection.py
│   ├── forecasting.py
├── README.md            # Project description
├── requirements.txt     # Python dependencies
