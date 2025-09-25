# Telco Customer Churn Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-0.24-green)
![XGBoost](https://img.shields.io/badge/XGBoost-1.7-orange)

## Overview
Predict customer churn for a telecom company using machine learning.  
Objectives:  
- Analyze customer behavior  
- Build predictive models  
- Identify key factors influencing churn  

## Dataset
Contains customer demographics, service usage, billing info, and churn status.  
- Target: `Churn` (1 = churned, 0 = retained)  
- Features include: tenure, contract type, services, monthly/total charges  

## Approach
1. **Data Cleaning**: Handle missing values, encode categorical variables  
2. **EDA**: Examine churn distribution and tenure patterns  
3. **Modeling**: LinearSVC, RandomForest, XGBoost  
4. **Imbalance Handling**: Oversampled minority class using SMOTE  
5. **Hyperparameter Tuning**: GridSearchCV for XGBoost  
6. **Feature Importance**: Identify key churn drivers  

## Key Insights
- Month-to-month contracts → higher churn  
- Customers without dependents or multiple lines → higher churn risk  
- Short tenure and higher charges → more likely to churn  

## Results
XGBoost with SMOTE and hyperparameter tuning achieved the best performance with improved recall and F1 score for churn prediction.  

## Requirements
- Python 3.x  
- pandas, seaborn, matplotlib  
- scikit-learn, xgboost, imbalanced-learn  

## Usage
```bash
git clone https://github.com/15kone/TelcoCustomerChurn
pip install -r requirements.txt
jupyter notebook
```
