# Classify-Customer-Churn


Predict customer churn using machine learning to help businesses retain valuable customers and reduce revenue loss.

---

##  Overview

Customer churn — when a customer leaves a service — is a major concern for subscription-based businesses. This project builds a machine learning model that classifies whether a customer is likely to churn, based on historical data from a telecommunications company.

Using a Random Forest Classifier, we identify key churn indicators such as tenure, monthly charges, and contract type, enabling proactive customer retention strategies.

---

##  Objective

Develop a supervised classification model to predict customer churn and provide insights into the key factors contributing to customer attrition.

---

##  Dataset Summary

- **Records**: 7,043 customers
- **Target Variable**: `Churn` (Yes/No)
- **Features**:
  - **Demographics**: Gender, Senior Citizen, Partner, Dependents
  - **Services**: Internet, Streaming, Security, Backup, etc.
  - **Billing**: MonthlyCharges, TotalCharges, PaymentMethod
  - **Account**: Tenure, Contract type, Paperless billing

---

## 🛠 Technologies Used

- Python 
- Pandas, NumPy
- Scikit-learn
- Seaborn & Matplotlib
- Jupyter Notebook

---

## ⚙ Process & Methodology

1. **Data Cleaning**  
   - Converted `TotalCharges` to numeric
   - Handled missing values
2. **Feature Encoding**  
   - Label encoding for categorical variables
3. **Feature Scaling**  
   - Standardized numerical columns
4. **Model Building**  
   - Used `RandomForestClassifier`
5. **Evaluation**  
   - Accuracy, Precision, Recall, F1-Score, Confusion Matrix
6. **Feature Importance Visualization**

---

##  Results

- **Accuracy**: ~79.7%
- **Precision**: 82.9% (No Churn), 66.2% (Churn)
- **Recall**: 91.2% (No Churn), 47.7% (Churn)
- **Top Predictors**: `tenure`, `MonthlyCharges`, `Contract`, `InternetService`

---

##  Key Insights

- Customers with **short tenure** are more likely to churn.
- **Month-to-month contracts** are associated with higher churn.
- Higher **monthly charges** often indicate dissatisfaction.

---

##  Business Impact

This model helps:
- Identify at-risk customers early
- Design targeted retention campaigns
- Reduce customer acquisition costs
- Improve overall customer lifetime value

---

##  Future Enhancements

- Hyperparameter tuning
- Handle class imbalance (e.g., SMOTE, weighted models)
- Try alternative models: XGBoost, Logistic Regression, etc.
- Use SHAP values for better explainability

---

## 📁 Project Structure

