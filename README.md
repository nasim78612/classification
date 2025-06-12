# Credit Default Risk Prediction – Machine Learning Capstone Project

## 📌 Project Overview
This project applies advanced machine learning techniques to predict credit default risk, ensuring more reliable financial decision-making. A structured approach optimizes feature selection, model tuning, and risk assessment methodologies, improving recall and precision.

## 🔍 Step-by-Step Process & Key Findings

### 1️⃣ Exploratory Data Analysis (EDA)
- **Data Overview & Cleaning:** 
  - Addressed missing values by adding an "Others" category for Education Level and Marital Status.
  - Removed duplicates and inconsistencies in financial attributes.
- **Outlier Detection & Transformation:** 
  - Used boxplots and Z-score analysis.
  - Applied cube root transformation to reduce skewness.
- **Feature Correlations:** 
  - Bill amounts across months showed strong positive correlations.
  - Higher credit limits correlated with lower default rates.
  - Repayment Status (September) strongly linked to default risk.

📊 **Impact:** A structured dataset makes predictive modeling more reliable.

### 2️⃣ Class Imbalance & Model Selection
- **Class Distribution Analysis:** Addressed imbalance due to more non-defaulters than defaulters.
- **SMOTE Implementation:** Generated synthetic minority-class samples, improving recall for defaulters.
- **Train-Test Split:** Applied an 80/20 split for efficient learning.
- **Final Model Choice:** XGBoost + SMOTE chosen for superior recall and F1-score.

📊 **Impact:** Balanced dataset improves financial risk predictions and reduces bias.

### 3️⃣ Model Optimization & Performance Evaluation
- **Hyperparameter Optimization:** Used Optuna (TPE algorithm) for tuning.
- **Evaluation Metrics:** Precision, Recall, F1-score, and Accuracy for balanced assessment.
- **Results Before & After Optimization:**
  
| Model & Dataset               | Accuracy | Precision (Class 1) | Recall (Class 1) | F1-Score (Class 1) |
|--------------------------------|----------|----------------------|-------------------|--------------------|
| XGBoost + SMOTE (Train)       | 91%      | 95%                  | 87%               | 91%                |
| XGBoost (Test Set - Original) | 79%      | 54%                  | 42%               | 48%                |
| After Tuning (Train)          | 91%      | 93%                  | 88%               | 91%                |
| Test Set with SMOTE (Experimental) | 82% | 87%                  | 76%               | 81%                |

📊 **Impact:** Fine-tuning strengthened recall, increasing defaulter detection accuracy while maintaining precision.

### 4️⃣ Model Explainability & Business Strategy
- **SHAP Analysis for Interpretability:** Explained how features influenced predictions.
- **Key Feature Insights:**
  - **Age:** Older individuals showed greater financial stability.
  - **Credit Limit:** Higher limits correlated with lower default risk.
  - **Repayment Status (Sep):** Delays in September strongly predicted defaults.
  - **Bill & Payment Amounts:** Spending trends influenced repayment risk.

📊 **Impact:** Improved trust in model decisions, helping banks refine lending strategies.

## 🚀 Final Conclusion & Business Implications
### ✅ Achievements:
- Successfully optimized credit default predictions using machine learning.
- Increased recall for defaulters, improving financial risk detection.
- Ensured model transparency using SHAP analysis.

### 📈 Next Steps:
- **Threshold Optimization:** Adjust cutoffs to enhance recall further.
- **Dynamic Credit Adjustments:** Implement adaptive lending policies based on risk assessment.
- **Automated Risk Monitoring:** Deploy real-time alerts for early detection.

🏆 **Overall Business Impact:**
✔ Improved risk assessment, reducing financial loss from defaults.  
✔ Balanced decision-making, minimizing false positives while maximizing recall.  
✔ Data-driven credit policies, ensuring sustainable profitability.  

🔗 **Author:** Nasim Aalam
📅 **Date:** June 2025  
