# AI-Risk-Fraud-Intelligence-Platform
AI Risk &amp; Fraud intelligence platform is a project created for my Data Science, Analytics and Artificial Inteligence Masters Degree. Its scope is to implement an end-to-end AI system that detects, scores, explains, and monitors suspicious financial activity using machine learning, anomaly detection, and deep learning techniques.(Built in Databricks)

# Project Overview

The AI Risk & Fraud Intelligence Platform is an end-to-end (production-inspired) machine learning system built entirely on Databricks Lakehouse architecture to detect, score, explain, and monitor suspicious financial transactions.

The platform combines:

* Supervised learning for known fraud patterns
  
* Anomaly detection for emerging and zero-day fraud

* Deep learning for sequential behavioral modeling

* Explainable AI (XAI) for regulatory transparency

* Monitoring & drift detection for long-term reliability

This project uses similar structures that modern fintech companies and digital banks implement for fraud detection systems leveraging distributed data processing and ML pipelines.


# Project Objectives

* Build a fintech AI system using Databricks

* Integrate multiple real-world fraud datasets into a unified Lakehouse schema

* Implement a hybrid detection engine (XGBoost + Random Forest + LSTM/Autoencoder)

* Deliver transparent risk scoring and explanations

* Simulate production monitoring & model governance


# System Architecture (Databricks Lakehouse)

The platform follows a layered Lakehouse architecture:

# 1. Data Ingestion Layer (Bronze)

* Raw dataset ingestion into Delta Tables

* Schema validation

* Metadata logging

# 2. Data Processing Layer (Silver)

* Cleaning & normalization

* Schema unification

* Feature standardization

* Missing value handling

# 3. Feature Store Layer (Gold)

* Transaction-level features

* User behavioral aggregates

* Device & identity features

* Temporal & velocity features

* Sequence embeddings

# 4. AI Intelligence Layer

* Supervised ML (XGBoost on Spark)

* Anomaly detection (Isolation Forest)

* Deep learning models (LSTM + Autoencoder with PyTorch on Databricks)

# 5. Risk Scoring & Explainability Layer

* Score fusion logic

* SHAP explanations

* Rationale behind code generation

# 6. Monitoring & Governance Layer

* Performance tracking

* Data drift detection

* Model versioning with MLflow

* Retraining triggers


# Data Ecosystem

The platform integrates four complementary datasets:

1. PaySim (Mobile Money Transactions):

* High-volume transaction simulation

* Balance changes

* Velocity feature generation

* Sequence modeling

2. Bank Account Fraud Dataset (NeurIPS 2022)

* Account-level fraud patterns

* Behavioral profiling

* Account takeover modeling

3. Financial Transactions Dataset

* Merchant & channel diversity

* Supervised baseline training

4. IEEE-CIS Fraud Detection Dataset

* Device fingerprinting

* Identity & session features

* Robust generalization testing

All datasets are stored and processed as Delta Lake tables within Databricks.

# Tech Stack 

Data & Processing

* Databricks Lakehouse

* Apache Spark (PySpark)

* Delta Lake

* SQL Analytics

Machine Learning

* Spark MLlib

* XGBoost

* Random Forest

* PyTorch (LSTM + Autoencoder)

* MLflow (experiment tracking)

Explainability

* SHAP

Serving & APIs

* Databricks Model Serving

* Databricks Jobs

Visualization

* Databricks SQL dashboards

# Key Features

Hybrid Detection Engine

* Distributed supervised learning

* Large-scale anomaly detection

* Sequence-based behavioral AI

Lakehouse Feature Store

* Centralized feature definitions

* Reusable training & inference features

Explainable AI

* SHAP-based local and global explanations

* Audit-ready reason codes

Risk Scoring Engine

* Weighted fusion of model outputs

* Risk tiers & decision logic

Monitoring & MLOps

* MLflow model registry

* Automated performance evaluation

* Drift detection using statistical tests


# Repository Structure

├── data/
│   ├── bronze/                 * Raw datasets
│   ├── silver/                 * Cleaned unified tables
│   └── gold/                   * Feature tables
│
├── notebooks/
│   ├── ingestion/
│   ├── preprocessing/
│   ├── feature_engineering/
│   ├── supervised_models/
│   ├── anomaly_detection/
│   ├── deep_learning/
│   ├── risk_scoring/
│   ├── explainability/
│   └── monitoring/
│
├── src/
│   ├── pipelines/
│   ├── models/
│   ├── scoring/
│   ├── explainability/
│   └── utils/
│
├── dashboards/
│   └── risk_monitoring.sql
│
├── mlflow/
│   └── experiments/
│
├── reports/
│   └── final_thesis.pdf
│
├── requirements.txt
└── README.md

# Author

Juan Ruiz
Master in Data Science, Analytics & Artificial Intelligence
Economist | Former Operations Manager

Specialization:
Fintech AI 
Fraud Detection
Risk Modeling
Distributed ML Systems
Databricks
