# 🩺 Diabetes Prediction Using Machine Learning

## 📌 Overview
Diabetes is a growing global health challenge, affecting millions of people and leading to severe complications such as heart disease, kidney failure, and vision loss. However, **early detection** can help in **preventing** or **managing diabetes effectively**.

This project utilizes **machine learning** to predict diabetes risk based on key health metrics and lifestyle factors. The model classifies individuals into three categories:
✅ **Healthy (No Diabetes)**  
⚠️ **Pre-Diabetic (Moderate Risk – Needs Lifestyle Changes)**  
🚨 **Diabetic (High Risk – Requires Medical Attention)**  

This predictive system can help **doctors**, **insurance providers**, and **individuals** take **proactive health measures** before complications arise.

---

## ❓ Problem Statement
Many individuals are unaware of their diabetes risk until serious symptoms appear. This project aims to answer:
- **Can we predict diabetes risk accurately using health data?**
- **What are the most influential factors contributing to diabetes?**
- **How can we use AI to support early detection and prevention?**

Using a dataset with **22 key health indicators**, this project analyzes risk factors such as **blood pressure, BMI, cholesterol levels, lifestyle habits, and family history** to predict diabetes.

---

## 📊 Dataset Overview
- **Number of Features:** 22 (including health metrics, lifestyle habits, and demographics)
- **Target Variable:** `Diabetes_012`
  - **0 → No Diabetes**
  - **1 → Pre-Diabetic**
  - **2 → Diabetic**
- **Why This Dataset?**
  - Covers both **medical** and **behavioral** risk factors.
  - Large sample size ensures **statistical reliability**.
  - No missing values, reducing data preprocessing efforts.

---

## 🔍 Key Findings from Data Analysis
During **Exploratory Data Analysis (EDA)**, we identified **key trends**:

✔ **BMI & Cholesterol Levels** – Strong correlation with diabetes risk.  
✔ **Physical Activity** – Individuals who exercise regularly have a **lower risk** of diabetes.  
✔ **Age & Gender** – Older individuals and males are at **higher risk**.  
✔ **Smoking & Heart Disease History** – Increases the likelihood of developing diabetes.  

📌 **Outlier Handling & Data Cleaning:**  
- Removed extreme values in **BMI** and **cholesterol** using statistical methods.  
- Checked for **highly correlated features** to remove redundancy.  

---

## 🛠 Feature Engineering – Improving the Model
To enhance model performance, we applied **advanced feature selection techniques**:

✅ **One-Hot Encoding:** Converted categorical data like **sex, education level, and income** into numerical format.  
✅ **Feature Scaling:** Applied **MinMax Scaling** to standardize BMI, blood pressure, and activity levels.  
✅ **Feature Selection:** Used **Recursive Feature Elimination (RFE)** to select the **10 most important features**.

---

## 🏆 Model Selection – Finding the Best Approach
We tested multiple machine learning models to identify the best one for **diabetes prediction**:

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|---------|------------|---------|-----------|
| **Logistic Regression** | 79% | 76% | 75% | 75% |
| **Decision Tree** | 84% | 82% | 81% | 81% |
| **Random Forest (Best Model)** ✅ | **89%** | **88%** | **87%** | **88%** |
| **K-Nearest Neighbors (KNN)** | 83% | 80% | 78% | 79% |

🚀 **Why Random Forest?**
- **Best Accuracy (89%)** – Outperforms other models.
- **Handles Non-Linearity** – Captures complex health patterns.
- **Feature Importance Insights** – Shows which factors contribute most to diabetes.

---

## 🏥 Real-World Business & Healthcare Applications
Our AI-based **diabetes risk prediction model** can be used in multiple sectors:

✔ **Hospitals & Clinics** – Helps doctors **detect high-risk patients early**, enabling timely intervention.  
✔ **Insurance Companies** – Assists in **assessing health risks**, allowing tailored insurance plans.  
✔ **Health Apps & Wearables** – Can be integrated into **smart health devices** to provide real-time risk scores.  
✔ **Public Health Policies** – Governments can use predictive insights to **target preventive healthcare campaigns**.  

**Potential Benefits:**
✅ Early detection saves lives.  
✅ Reduced healthcare costs.  
✅ Personalized health recommendations.  
