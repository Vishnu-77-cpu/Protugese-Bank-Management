![WhatsApp Image 2025-11-23 at 16 58 30_01827c85](https://github.com/user-attachments/assets/03a08898-7340-43b4-9536-649aa288f891)

🏦 Portuguese Bank Marketing Campaign – End-to-End Data Science Project
🔍 EDA • Feature Engineering • SMOTE • Machine Learning • XGBoost
<p align="center"> <img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge" /> <img src="https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge" /> <img src="https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge" /> <img src="https://img.shields.io/badge/Model-XGBoost-orange?style=for-the-badge" /> </p>
📌 Project Description

This project analyzes the Portuguese Bank Marketing Dataset to understand customer behavior during marketing campaigns and predict whether a customer will subscribe to a term deposit.

It includes complete EDA, feature engineering, data transformation, class imbalance handling, model building, and business insights.

This project is ideal for:

Data Science Portfolio

ML Engineering Practice

Marketing Analytics

Predictive Modeling

🎯 Project Objectives
Task 1 — Complete Data Analysis Report

Clean and analyze customer, campaign, and economic data

Identify key factors affecting customer subscription

Visualize distributions, correlations, outliers, and patterns

Task 2 — Predictive Modeling

Handle class imbalance using SMOTE

Train 5 ML models (LR, DT, RF, XGBoost, LightGBM)

Compare recall, precision, F1, and AUC

Select the best model for customer prediction

Task 3 — Business Recommendations

Provide actionable strategies for improving conversions

Recommend customer segments & optimal campaign timings

Suggest contact methods & call frequency improvements

📁 Dataset Overview

Source: Portuguese Bank

Duration: 2008–2010

Rows: 41,000+

Target: y (yes/no → term deposit subscribed)

Data Includes:

Customer attributes (age, education, job, loans)

Contact method & call details

Campaign history

Macro-economic indicators

🛠️ Technologies & Libraries Used

Python

Pandas, NumPy

Matplotlib, Seaborn

Scikit-Learn

XGBoost, LightGBM

SMOTE (imblearn)

Statsmodels (VIF Analysis)

🔍 Key EDA Insights
✔ Customer Behavior

Middle-aged customers (30–60) subscribe more

Higher education & stable job roles show better engagement

✔ Contact Findings

Cellular contact performs far better than telephone

May, June, July months show higher success

✔ Economic Impact

Lower interest rates (euribor3m) → higher subscriptions

Strong correlations found among economic indicators

✔ Data Challenges

High imbalance (~11% YES)

Outliers in campaign counts & duration

Skewed features requiring log transformation

🧠 Machine Learning Models Used
Model	Status	Notes
Logistic Regression	✔	High accuracy, low recall
Decision Tree	✔	Overfitting
Random Forest	✔	Good stability
XGBoost	⭐ Best Model	Best recall & F1-score
LightGBM	✔	High accuracy
📊 Model Performance Summary
Model	Accuracy	Precision (Yes)	Recall (Yes)	F1 (Yes)
LightGBM	0.9006	0.61	0.34	0.43
XGBoost	0.8969	0.56	0.38	0.45
Random Forest	0.8862	0.49	0.38	0.43
Decision Tree	0.8413	0.32	0.36	0.34
Logistic Regression	0.9000	0.62	0.26	0.36
🎉 Final Selected Model: XGBoost

The XGBoost model provides the best recall and F1-score for identifying potential term-deposit subscribers, making it the most suitable for the bank’s real-world marketing needs.

💡 Business Recommendations
✔ 1. Target High-Probability Customers

Use the model's prediction scores to prioritize customers who are most likely to subscribe.

✔ 2. Prefer Mobile (Cellular) Calls

Customers respond much better to mobile communication than landline calls.

✔ 3. Limit Calls to 2–3 Attempts

Excessive calling reduces customer interest; optimal follow-up: 2–3 calls.

✔ 4. Leverage Previous Success

Customers with positive outcomes in past campaigns should be contacted first.

✔ 5. Time Campaigns Wisely

Launch campaigns during favorable economic conditions (e.g., low interest rates).

✔ 6. Improve Call Quality

Longer, more meaningful conversations increase subscription probability.
