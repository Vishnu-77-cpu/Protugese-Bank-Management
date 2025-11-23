![WhatsApp Image 2025-11-23 at 16 58 30_01827c85](https://github.com/user-attachments/assets/03a08898-7340-43b4-9536-649aa288f891)

 Portuguese Bank Marketing Campaign – End-to-End Data Science Project
 EDA • Feature Engineering • SMOTE • Machine Learning Models • XGBoost

Project Overview

This project analyzes the Portuguese Bank Marketing Dataset to understand customer behaviors during marketing campaigns and build a predictive model that identifies which customers are most likely to subscribe to a term deposit.

The goal is to support the bank’s marketing team in making data-driven decisions, reduce unnecessary calls, target the right customers, and improve overall conversion rates.

Objectives
Task 1 – Complete Data Analysis Report

Perform data cleaning, preprocessing, and exploratory data analysis

Understand customer, campaign, and economic patterns

Identify key factors influencing term deposit subscriptions

Task 2 – Predictive Modeling

Build ML models that can classify customers into “Will Subscribe” or “Will Not Subscribe”

Handle class imbalance using SMOTE

Compare multiple models and select the best performer

Task 3 – Business Recommendations

Provide actionable insights for the bank marketing team

Suggest strategies to increase customer conversions

Dataset

Portuguese Bank Marketing Dataset (May 2008 – November 2010)
Includes:

Customer attributes (age, job, education, loans, marital status)

Campaign data (contact type, duration, month, previous outcome)

Economic indicators (euribor3m, emp.var.rate, cons.price.idx, nr.employed)

Target: y (yes/no – subscribed)

Tech Stack & Libraries

Python, Pandas, NumPy – Data Cleaning

Matplotlib, Seaborn – EDA Visualizations

Scikit-learn – ML Models, Preprocessing, SMOTE

XGBoost, LightGBM – Advanced boosting models

VIF Analysis – Multicollinearity check

Exploratory Data Analysis (Highlights)
Class Imbalance

88–90% “No”, only ~11% “Yes”

✔ Important Patterns

Cellular contact works better than telephone

Middle-aged & educated customers subscribe more

Favourable economic conditions increase subscription success

Longer, meaningful conversations increase chance of “Yes”

Previous successful campaigns strongly affect future success

✔ Data Cleaning

Removed duplicates

Treated 'unknown' values

Corrected skewness using log transformations

Removed duration feature due to target leakage

Feature Engineering

Handled skewed features: campaign, previous, duration

One-hot encoding for categorical features

StandardScaler for numerical columns

Removed multicollinear features for Logistic Regression

Applied SMOTE to balance minority class

Machine Learning Models Used
Model	Status

Logistic Regression	✔ Used
Decision Tree	✔ Used
Random Forest	✔ Used
XGBoost	⭐ Best Model
LightGBM	✔ Tuned

Model Performance Summary
Model	Accuracy	Precision (Yes)	Recall (Yes)	F1 (Yes)
LightGBM	0.9006	0.61	0.34	0.43
XGBoost	0.8969	0.56	0.38	0.45
Random Forest	0.8862	0.49	0.38	0.43
Decision Tree	0.8413	0.32	0.36	0.34
Logistic Regression	0.9000	0.62	0.26	0.36
✅ Final Model Selected: XGBoost

XGBoost provides the best balance between recall and F1-score for the YES class — the most important for the bank.

Business Recommendations
1️⃣ Target the Right Customers

Use the model to call high-probability customers first → higher conversions & lower cost.

2️⃣ Use Cellular Over Telephone

Mobile calls produce significantly higher positive responses.

3️⃣ Limit Contact Attempts

2–3 calls per customer work best — avoid over-calling.

4️⃣ Retarget Customers with Previous Success

Past successful outcomes strongly indicate future success.

5️⃣ Focus on Educated & Stable Job Profiles

Higher education and stable professions show higher subscription rates.

6️⃣ Time Campaigns During Favourable Economic Conditions

Low interest rates → more customers invest in term deposits.

7️⃣ Improve Call Quality

Longer, meaningful calls increase success. Train agents accordingly.
