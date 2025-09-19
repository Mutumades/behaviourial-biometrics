🧠 Behavioral Biometric Fraud Detection — Kenya

Post-Login AI Security for Mobile Banking

🌍 Overview

This project builds an AI-powered behavioral biometric security system to detect fraudulent sessions after login in mobile banking apps.

Unlike traditional security (PINs, OTPs, facial/ fingerprint login), this system monitors how users behave during the session — their:

🖐️ Touch dynamics

⌨️ Typing patterns

🧭 Navigation flow

📍 Context (location, time, SIM, device, network)

It can catch attackers who bypass login using Artificial Intelligence deepfakes, stolen OTPs, or remote access tools.

⚠️ Fraud Types Detected

The system simulates and detects 5 major fraud categories common in Kenya and Africa:

Fraud Type	Description
SIM-Swap Fraud	Criminal hijacks the victim’s phone number to intercept OTPs
Remote Access Fraud (RAT)	Fraudster remotely controls the victim’s phone and drains funds
Social Engineering Scams	Victims are tricked into sending money to fraudsters
Bot-like Behavior	Automated scripts mimic human behavior to steal funds fast
High-Value Mule Transfers	Sudden large transfers far beyond a user’s normal behavior
🧪 Dataset

Synthetic behavioral biometrics dataset of 700 users

~25–45 sessions each (heavy-tailed distribution)

~5% labeled fraud

Includes touch, typing, navigation, and context data

Realistic fraud behaviors injected (SIM/device swaps, remote flows, bots, outlier amounts)

⚡ This approach is ethical and realistic — real behavioral banking data is private and unavailable, so synthetic data is required for safe experimentation.

⚙️ Tech Stack

Python, pandas, scikit-learn, xgboost

matplotlib and seaborn for analysis & visualizations

Streamlit + pyngrok for real-time fraud detection dashboard

Google Colab for development

📊 Results
Model	Accuracy	Precision	Recall	F1	ROC-AUC
Logistic Regression	92.6%	99.3%	92.9%	96.0%	0.941
Random Forest	97.9%	97.9%	99.9%	98.9%	0.957
XGBoost	98.6%	98.7%	99.8%	99.2%	0.964

✅ XGBoost was selected as the final model for deployment due to its high recall and low false positives.
📌 High recall ensures almost all fraud is caught while minimizing false alarms.

💻 Dashboard (Streamlit)

A live demo dashboard lets users:

📝 Score single sessions manually

📁 Upload CSV files for batch scoring

🎚️ Adjust the fraud decision threshold

📊 View fraud probabilities and top feature importances

This proves the system works beyond notebooks — in real-time.
