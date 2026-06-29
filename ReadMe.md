# Operational End-to-End Fraud Detection Pipeline

[![Quantinar CourseLet](https://img.shields.io/badge/Quantinar-QuantLet-blue)](https://quantinar.com)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/)
[![Streamlit App](https://img.shields.io/badge/Data%20App-Streamlit-FF4B4B.svg)](https://streamlit.io)

An end-to-end machine learning solution designed to identify fraudulent financial transactions in highly imbalanced environments. Developed by **SINGH** and **HAERDLE** (2026) for the *Institute for Digital Assets (IDA)*, this project shifts the focus from standard academic metrics to operational, business-first deployment.

---

## 📌 Project Overview

In financial fraud detection, standard accuracy is a misleading metric due to extreme class imbalance. This project tackles a dataset of **6.3 million transactions** containing an operational fraud rate of just **0.13%**. 

Instead of optimizing for raw accuracy, this pipeline optimizes the **Precision-Recall AUC**, establishing a custom classification threshold of **0.91** to drastically minimize false alarms while capturing critical fraudulent activity.

### Key Features
* **Imbalance Resolution**: Advanced data handling and algorithm-level weighting using XGBoost.
* **Operational Thresholding**: Finely tuned classification boundary (0.91) to balance investigator workload (Precision) with risk mitigation (Recall).
* **Interactive Inference App**: A live Streamlit interface built for fraud analysis teams to evaluate individual transactions instantly.

---

## 🛠️ Tech Stack & Dependencies

* **Language**: Python 3.10+
* **Core ML Stack**: XGBoost, Scikit-Learn
* **Data Manipulation**: Pandas, NumPy
* **Model Serialization**: Joblib
* **Deployment UI**: Streamlit

---

## 📂 Repository Structure

```text
├── analysis_model.ipynb          # EDA, feature engineering, and model training
├── fraud_detection_app.py       # Streamlit web application script
├── fraud_detection_pipeline.joblib # Serialized production-ready ML pipeline
├── metainfo.txt                 # Quantinar QuantLet metadata configuration
└── README.md                    # Project documentation