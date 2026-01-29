# Customer Churn Prediction Project

## Overview
This project is a personal data science initiative focused on the banking sector. The goal is to predict customer attrition (churn) using machine learning. By analyzing customer demographics and financial behavior, we aim to identify the key factors that influence a customer's decision to leave the bank.

## Task Objective
The primary objective is to build a predictive model that identifies customers likely to churn.
**Key Goals:**
1.  Clean and preprocess the "Churn Modelling" dataset.
2.  Encode categorical features (Geography, Gender) into numerical format.
3.  Train a classification model (Random Forest) to predict churn.
4.  Analyze **Feature Importance** to interpret the model's decision logic.

## Approach
The project was executed using Python in a Jupyter Notebook environment:

1.  **Data Preparation:**
    * Dropped non-predictive columns (`RowNumber`, `CustomerId`, `Surname`) to reduce noise.
    * Verified data integrity by checking for missing values.

2.  **Feature Engineering:**
    * **Label Encoding:** Applied to the binary `Gender` column.
    * **One-Hot Encoding:** Applied to the nominal `Geography` column (France, Germany, Spain) to ensure mathematical correctness without introducing ordinal bias.

3.  **Model Training:**
    * Utilized a **Random Forest Classifier**, a robust ensemble method chosen for its high accuracy and ability to provide interpretable feature importance scores.
    * Split data into 80% training and 20% testing sets.

## Results and Insights
* **Predictive Power:** The Random Forest model achieved a high accuracy (approx. 87%), effectively identifying potential churners.
* **Feature Importance Analysis:**
    * **Age** was identified as the strongest predictor of churn.
    * **Number of Products** and **Account Balance** were also critical factors.
    * **Balance** Account balance also plays a major role.
    
These insights imply that retention strategies should be personalized based on customer age and product engagement levels.
