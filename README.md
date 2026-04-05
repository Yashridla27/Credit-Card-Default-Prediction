# Credit Card Default Prediction using Machine Learning

## Project Overview
This project predicts whether a customer will default on their credit card payment. The objective is to help financial institutions identify high-risk customers and reduce financial losses.

---

## Dataset
- Source: Credit Card Default Dataset  
- Features include demographic details, bill amounts, and payment history  
- Target Variable: Default (Yes/No)

---

## Data Preprocessing
- Metadata inspection and column validation  
- Removed duplicate records  
- Created Data Audit Report including:
  - Mean, Median, Std, Variance  
  - Percentiles (P1, P5, P10, P25, P50, P75, P90, P95, P99)  
- Applied Label Encoding  
- Standardized numerical features  

---

## Feature Engineering
- Removed multicollinearity using VIF  
- Selected important features using RFE  

---

## Handling Imbalanced Data
- Used Class Weights  
- Applied SMOTE  
- Selected best approach based on performance  

---

## Models Used
- Logistic Regression  
- KNN  
- Naive Bayes  
- Decision Tree
- Random Forest   
- SVM  
- XGBoost  
- LightGBM  
- CatBoost  

---

## Model Selection
- Selected models based on **Accuracy + Recall**  
- Best Models:
  - CatBoost (Best)  
  - LightGBM (Second Best)  

---

## Hyperparameter Tuning
- Applied GridSearchCV on CatBoost and LightGBM  

---

## Ensemble Model
- Combined CatBoost + LightGBM (Heterogeneous Model)  
- Achieved slight improvement in performance  

---

## Model Evaluation

### Confusion Matrix
![Confusion Matrix](images/confusion_matrix.png)

### Model Comparison
![Model Comparison](images/model_comparison.png)

---

## Final Results
- Accuracy: ~77%  
- Balanced Recall across classes  
- Robust performance on imbalanced dataset  

---

## Model Saving
- Saved final model using Joblib (`pipeline_main1.pkl`)  

---

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Scikit-learn  
- CatBoost, LightGBM, XGBoost  
- Matplotlib, Seaborn  

---
