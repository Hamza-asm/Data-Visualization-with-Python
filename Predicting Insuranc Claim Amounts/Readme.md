# Medical Insurance Cost Prediction

## Overview
This project is a personal data science study focused on the healthcare/insurance domain. The goal is to apply regression analysis to estimate the medical insurance costs for individuals based on their personal health data.

## Task Objective
The primary objective is to predict the continuous variable `charges` (medical costs).
**Key Goals:**
1.  Analyze the "Medical Cost Personal Dataset" to understand feature distributions.
2.  Visualize the impact of key health indicators (BMI, Age, Smoking) on costs.
3.  Train a **Linear Regression** model to quantify these relationships.
4.  Evaluate the model's prediction error using MAE and RMSE.

## Approach
The analysis was conducted in a Jupyter Notebook using Python:

1.  **Data Preprocessing:**
    * Cleaned the dataset by removing duplicates.
    * **Label Encoding:** Converted `sex` and `smoker` to binary format (0/1).
    * **One-Hot Encoding:** Applied to the `region` column to treat it as a nominal variable.

2.  **Exploratory Data Analysis (EDA):**
    * **Box Plot:** Used to contrast the drastic difference in charges between smokers and non-smokers.
    * **Scatter Plots:** Visualized the correlation between BMI and Charges, revealing a strong interaction effect where high BMI combined with smoking results in the highest costs.

3.  **Model Training:**
    * Implemented a standard **Linear Regression** model using Scikit-Learn.
    * Split the data (80/20) to ensure fair evaluation on unseen data.

## Results and Insights
* **The Smoking Factor:** Smoking status is the single most significant predictor of high insurance charges. Smokers pay significantly more than non-smokers regardless of other factors.
* **BMI Interaction:** The impact of BMI on charges is not uniform; it is much more severe for smokers.
* **Model Accuracy:** The Linear Regression model performed well, providing a baseline for cost estimation.
    * **MAE:** The average prediction error (in dollars).
    * **RMSE:** The root mean squared error, accounting for large outliers.
