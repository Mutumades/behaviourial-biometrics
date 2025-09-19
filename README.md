Capstone project 

Project Overview

Detects mobile banking fraud after login using behavioral biometrics

Catches SIM-swap, remote access, social engineering, bot-like, and high-value mule fraud

Uses a synthetic dataset of 700 users (~5% fraud)

Provides a working Streamlit dashboard for real-time session scoring

Repository Contents

notebooks/Behaviourial_Biometric_Security_System.ipynb — full Google Colab code (data prep → models → dashboard)

models/ — trained model + preprocessing pipeline (to be added)

app/ — dashboard code (to be added)

Model Results
Logistic Regression — Accuracy: 92.6%, Precision: 99.3%, Recall: 92.9%, F1: 96.0%, ROC-AUC: 0.941
Random Forest — Accuracy: 97.9%, Precision: 97.9%, Recall: 99.9%, F1: 98.9%, ROC-AUC: 0.957
XGBoost — Accuracy: 98.6%, Precision: 98.7%, Recall: 99.8%, F1: 99.2%, ROC-AUC: 0.964

Author
Desmond Mutuma
