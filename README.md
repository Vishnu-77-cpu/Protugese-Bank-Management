<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/a6ab9314-465e-4502-894e-b0a13c8c9a1b" />

---

## 🎯 **Project Objectives**

### **Task 1 — Complete Data Analysis Report**
- Clean and analyze customer, campaign, and economic data  
- Identify key factors affecting customer subscription  
- Visualize distributions, correlations, outliers, and patterns  

### **Task 2 — Predictive Modeling**
- Handle class imbalance using **SMOTE**  
- Train 5 ML models (LR, DT, RF, XGBoost, LightGBM)  
- Compare recall, precision, F1, and AUC  
- Select the best model for customer prediction  

### **Task 3 — Business Recommendations**
- Provide actionable strategies for improving conversions  
- Recommend optimal campaign timing and customer targeting  
- Suggest best contact methods and call frequency  

---

## 📁 **Dataset Overview**

- **Source:** Portuguese Bank  
- **Duration:** 2008–2010  
- **Rows:** 41,000+  
- **Target:** `y` (yes/no → term deposit subscribed)

### **Dataset Includes:**
- Customer attributes (age, education, job, loans)  
- Contact method & call details  
- Campaign history  
- Macro-economic indicators  

---

## 🛠️ **Technologies & Libraries Used**

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-Learn  
- XGBoost, LightGBM  
- SMOTE (imblearn)  
- Statsmodels (VIF Analysis)

---

## 🔍 **Key EDA Insights**

###  **Customer Behavior**
- Middle-aged customers (30–60) subscribe the most  
- Higher education & stable job roles show better engagement  

###  **Contact Findings**
- Cellular contact performs far better than telephone  
- May, June, July are the strongest months  

###  **Economic Impact**
- Lower interest rates (euribor3m) correlate with higher subscriptions  
- Strong correlations found among economic indicators  

###  **Data Challenges**
- High imbalance (~11% YES)  
- Outliers in campaign counts & duration  
- Skewed features requiring log transformation  

---

## 🧠 **Machine Learning Models Used**

| **Model** | **Status** | **Notes** |
|----------|------------|-----------|
| Logistic Regression | ✔ | High accuracy, low recall |
| Decision Tree | ✔ | Overfitting |
| Random Forest | ✔ | Good stability |
| **XGBoost** | ⭐ **Best Model** | Best recall & F1 |
| LightGBM | ✔ | High accuracy |

---

## 📊 **Model Performance Summary**

| **Model**              | **Accuracy** | **Precision (Yes)** | **Recall (Yes)** | **F1 (Yes)** |
|------------------------|--------------|----------------------|-------------------|--------------|
| **LightGBM**           | **0.9006**   | 0.61                 | 0.34              | 0.43         |
| **XGBoost**            | 0.8969       | 0.56                 | **0.38**          | **0.45**     |
| **Random Forest**      | 0.8862       | 0.49                 | 0.38              | 0.43         |
| **Decision Tree**      | 0.8413       | 0.32                 | 0.36              | 0.34         |
| **Logistic Regression**| 0.9000       | 0.62                 | 0.26              | 0.36         |

---

## 🎉 **Final Selected Model: XGBoost**

XGBoost provides the **best balance of recall and F1-score** for identifying potential subscribers, making it the most practical choice for real-world marketing campaigns.

---

## 💡 **Business Recommendations**

###  **1. Target High-Probability Customers**
Use model predictions to focus on customers with higher subscription likelihood.

###  **2. Prefer Mobile (Cellular) Calls**
Cellular communication shows far better conversion rates than telephone.

###  **3. Limit Calls to 2–3 Attempts**
Avoid excessive calling; optimal follow-up is 2–3 attempts.

###  **4. Leverage Previous Campaign Success**
Customers with successful past outcomes should be prioritized.

###  **5. Time Campaigns Wisely**
Campaigns perform better during favorable economic conditions (e.g., low interest rates)

###  **6. Improve Call Quality**
Longer, meaningful conversations increase the chance of subscription.

---


