# 🌍 Air Quality Time-Series Analytics, Forecasting & Anomaly Detection

An end-to-end Data Science project that analyzes environmental sensor data using Time Series Analysis, Feature Engineering, Machine Learning, and Anomaly Detection techniques.

The project predicts future Carbon Monoxide (CO) pollution levels and detects abnormal sensor behavior using historical air quality measurements.

---

## 📌 Project Overview

This project builds a complete machine learning workflow for environmental data analytics.

Main objectives:

- Analyze hourly air quality measurements
- Detect abnormal sensor behavior
- Forecast future CO concentration
- Support environmental monitoring through predictive analytics

---

## 🚀 Key Features

- Time Series Analysis
- Data Cleaning & Preprocessing
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Anomaly Detection (Isolation Forest)
- CO Forecasting (Random Forest)
- Hyperparameter Tuning (GridSearchCV)
- TimeSeriesSplit Cross Validation
- Feature Importance Analysis

---

## 🛠 Tech Stack

**Programming**

- Python

**Libraries**

- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

**Machine Learning**

- Random Forest
- Isolation Forest
- GridSearchCV
- TimeSeriesSplit

---

## 📊 Dataset

**Source:** UCI Machine Learning Repository – Air Quality Dataset

The dataset contains hourly environmental measurements collected from an air quality monitoring station in Italy, including:

- CO
- NOx
- NO2
- Temperature
- Humidity
- Air Quality Sensor Measurements

---

## ⚙ Machine Learning Workflow

### Data Cleaning

- Replaced invalid sensor readings (-200)
- Interpolated missing values
- Created Datetime index

### Feature Engineering

- Time Features
- Lag Features
- Rolling Statistics
- Difference Features

### Anomaly Detection

Isolation Forest

### Forecasting

Random Forest Classifier

### Model Optimization

- GridSearchCV
- TimeSeriesSplit

---

## 📈 Model Evaluation

Performance evaluated using:

- Accuracy
- ROC-AUC
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve
- Feature Importance

---

## 📂 Repository Structure

```text
Air-Quality-Forecasting-Anomaly-Detection/
│
├── README.md
├── requirements.txt
│
├── data/
│   └── AirQualityUCI.csv
│
├── notebooks/
│   └── Air_Quality_Forecasting.ipynb
│
└── images/
```

---

## 🚀 Installation

```bash
git clone https://github.com/farmaieshi/Air-Quality-Forecasting-Anomaly-Detection.git

cd Air-Quality-Forecasting-Anomaly-Detection

pip install -r requirements.txt
```

---

## ▶️ Run

```bash
jupyter notebook
```

Open:

```
notebooks/Air_Quality_Forecasting.ipynb
```

---

## 🔮 Future Improvements

- XGBoost / LightGBM
- LSTM Forecasting
- Streamlit Dashboard
- Explainable AI (SHAP)
- Real-time Air Quality Monitoring
