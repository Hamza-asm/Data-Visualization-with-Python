# Personal Loan Acceptance Prediction

## Overview
This project applies machine learning to the banking sector to optimize marketing campaigns. By analyzing historical campaign data, the goal is to predict which customers are likely to accept a personal loan (term deposit) offer, allowing for more targeted and efficient marketing strategies.

## Task Objective
The primary objective is to solve a binary classification problem: Will the customer subscribe? (Yes/No).
**Key Goals:**
1.  Explore the "Bank Marketing" dataset to understand customer demographics.
2.  Visualize the relationship between Job, Marital Status, and Loan Acceptance.
3.  Train a **Decision Tree Classifier** to predict customer response.
4.  Evaluate the model using Accuracy and Confusion Matrix.

## Approach
The solution was implemented using Python in a Jupyter Notebook:

1.  **Data Analysis (EDA):**
    * **Job Analysis:** Visualized acceptance rates across different professions.
    * **Demographics:** Analyzed the age distribution and marital status of potential borrowers.

2.  **Data Preparation:**
    * Used **One-Hot Encoding** to transform categorical variables (e.g., `job`, `marital`, `education`) into a machine-readable numeric format.
    * Encoded the target variable (`deposit`) into binary 0/1.

3.  **Model Training:**
    * Implemented a **Decision Tree Classifier** (`max_depth=5`).
    * Split the dataset into training and testing sets (80/20 split) to validate performance.

## Results and Insights
* **Target Audience:** The analysis suggests that specific groups (e.g., retired individuals and students) have higher engagement rates compared to blue-collar workers.
* **Model Accuracy:** The model performed well, achieving an accuracy of approximately **80%+**, providing a reliable baseline for filtering potential leads.
* **Strategic Value:** By deploying this model, a bank could reduce call center costs by focusing only on customers with a high predicted probability of acceptance.