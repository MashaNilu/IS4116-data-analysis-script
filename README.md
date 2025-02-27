# Placement Analysis - Factors Affecting Campus Placement

## 📌 Overview

This project analyzes factors influencing campus placements using **data analytics and machine learning techniques**. The dataset includes students' academic records, work experience, specializations, and placement outcomes. The goal is to uncover insights into placement trends and predict salary outcomes using statistical modeling.

## 📊 Key Objectives

- Identify key factors influencing **placement status**.
- Analyze the impact of **academic scores, work experience, and specialization**.
- Predict **placement likelihood** using **Logistic Regression**.
- Predict **salary for placed students** using **Linear Regression**.
- Visualize trends using **Matplotlib & Seaborn**.

## 📂 Dataset

- **Source:** Kaggle Dataset ("Factors Affecting Campus Placement")
- **File:** `Placement_Data_Full_Class.csv`
- **Key Features:**
  - `ssc_p`, `hsc_p`, `degree_p`, `mba_p`: Academic Scores
  - `workex`: Work Experience (Yes/No)
  - `specialisation`: MBA Specialization
  - `status`: Placement Status (Placed/Not Placed)
  - `salary`: Salary (for placed students)

## 🔍 Exploratory Data Analysis (EDA)
- **Placement Rate by MBA Score:** Higher MBA scores correlate with better placement rates.
- **Placement Rate by Work Experience:**
  - **No Experience:** ~60% placement rate.
  - **With Experience:** >85% placement rate.
- **Salary Trends:**
  - Marketing & HR specialization has higher median salaries.
  - Science & Technology degrees lead to better salaries.

## 🛠️ Technologies Used
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn
- **Machine Learning Models:** Logistic Regression, Linear Regression

## 📈 Machine Learning Models
### **Placement Prediction (Logistic Regression)**
- **Accuracy:** ~80%
- **Key Factors Affecting Placement:** Work Experience, Degree Type, MBA Score

### **Salary Prediction (Linear Regression)**
- **MSE:** High (due to missing salary-related factors)
- Salary Prediction Approach

Initial Attempts: Linear Regression, Decision Trees, Random Forest, and XGBoost all performed poorly due to missing key salary-related factors.

Filtered Approach: We attempted predicting salary separately for Science & Technology and Commerce & Management students.

Results: R² scores did not significantly improve, indicating that salary prediction remains difficult with the available features.

Key Observations:

Salary likely depends on external factors not present in the dataset (e.g., job role, company reputation, industry demand).

Degree specialization alone is not a strong predictor of salary.

## 📜 How to Run the Project
1. Clone the repository:
   ```bash
   git clone [Your GitHub Repo Link]
   cd placement-analysis
   ```
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```
3. Run the Python script:
   ```bash
   python analysis.py
   ```
4. View results in the generated **visualizations and model outputs**.




## 📌 License
This project is licensed under the MIT License.

