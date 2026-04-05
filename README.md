# Card Default Prediction using Machine Learning

## Project Overview
This project predicts whether a customer will default on their credit card payment. The objective is to help financial institutions identify high-risk customers and reduce financial losses.

---

## Dataset
- Source: Credit Card Default Dataset  
- Features include demographic details, bill amounts, and payment history  
- Target Variable: Default (Yes/No)
  
### Dataset File
You can find the dataset used in this project here:

- <a href="https://github.com/Yashridla27/Credit-Card-Default-Prediction/blob/main/default_of_credit_card_clients.xls">Download Dataset</a>

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
- Confusion Matrix visualization is based on the CatBoost model (best individual performer)
<img width="683" height="568" alt="Screenshot 2026-04-05 214957" src="https://github.com/user-attachments/assets/165d766c-3d0a-4939-84e3-8b50fcb1d061" />

### Model Comparison
- Model comparison is based on the top-performing models: LightGBM, CatBoost, and the final heterogeneous ensemble model
<img width="863" height="584" alt="Screenshot 2026-04-05 214930" src="https://github.com/user-attachments/assets/6e3a6479-d3eb-4c6a-91b5-ef56180d419f" />

---

## Final Results
- Final Model: Heterogeneous Ensemble Model (CatBoost + LightGBM)
- Accuracy: ~77%  
- Balanced Recall across classes  
- Robust performance on imbalanced dataset  

---

## 📓 Project Notebook

You can view the full implementation here:

- <a href="https://github.com/Yashridla27/Credit-Card-Default-Prediction/blob/main/Credit-Card-Default-Prediction%20.ipynb">View Full Project Notebook</a>

---

## Model Saving
Saved final model using Joblib 

- <a href="https://github.com/Yashridla27/Credit-Card-Default-Prediction/blob/main/pipeline_main1.pkl">Final Machine Learning Model</a>

---

## Tools & Technologies
- Python  
- Pandas, NumPy  
- Scikit-learn  
- CatBoost, LightGBM, XGBoost  
- Matplotlib, Seaborn  

---
