# Diabetes Prediction Using the Pima Indian Dataset  
### A Comparative Analysis of Logistic Regression, OLS, and Decision Trees

## 📋 Project Overview

This project explores various statistical and machine learning models to predict diabetes outcomes using the **Pima Indian Diabetes dataset**. The primary goal is to identify which physiological features most influence the likelihood of diabetes and to compare model performance for clinical risk prediction.

> Originally completed as a class project by Trent Yu and Izabella Orozco.

---

## 🧬 Dataset Summary

- **Source**: UCI Machine Learning Repository
- **Observations**: 768
- **Features (X)**:
  - Pregnancies
  - Glucose
  - Blood Pressure
  - Skin Thickness
  - Insulin Level
  - BMI
  - Diabetes Pedigree Function
  - Age
- **Target (y)**: `Outcome` — 1 if diabetic, 0 if not

- **A coreelation heatmap**:
  ![Screenshot 2025-06-05 at 15 56 28](https://github.com/user-attachments/assets/4dc8134f-84b0-4a46-8e1f-0353191ecaeb)



---

## ⚙️ Methods Used

1. **Logistic Regression**  
   - Estimated odds ratios for key features  
   - Glucose had the highest influence on predicted probability  
   - Interpretable and widely used in clinical settings

2. **Multiple Linear Regression (OLS)**  
   - Used to understand linear relationships and contribution of features  
   - Identified Glucose, Pregnancies, and BMI as statistically significant predictors

3. **Decision Tree & Random Forest**  
   - Non-linear modeling with automatic feature selection  
   - Glucose identified as the root node in decision tree  
   - Accuracy improved through pruning and ensemble averaging

---

## 📈 Results Summary

| Model                  | Accuracy | Precision | Notable Insight            |
|------------------------|----------|-----------|----------------------------|
| Logistic Regression    | ~0.746   | ~0.695    | Glucose strongly predictive |
| OLS Regression         | N/A      | N/A       | Glucose & BMI are key      |
| Random Forest (after tuning) | ~0.76    | N/A       | Root node = Glucose         |

- Glucose was consistently the **most impactful predictor** across all models.
- Pairplots revealed moderate linear correlation between Glucose and Outcome.

---

## 🧪 Tools & Libraries

- Python (Pandas, NumPy, Seaborn, Scikit-learn, Statsmodels)
- Jupyter Notebook
- Matplotlib for visualization

---

## 📁 Files Included

- `Pima_Indians_Diabetes.ipynb`: Main analysis notebook
- `Pima Indian Diabetes Analysis Presentation.pdf`: Summary slides

---

## 🧭 Future Improvements

- Apply SMOTE or resampling techniques to handle class imbalance
- Use ROC curves and AUC for better model evaluation
- Implement more advanced models like XGBoost or SVM

---

## 📌 Disclaimer

This project is for academic purposes using open-access, anonymized data. It is not intended to provide clinical recommendations or medical diagnoses.
