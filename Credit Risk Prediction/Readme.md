# Credit Risk Prediction Project

## Overview
This project focuses on building a machine learning model to automate the loan approval process. By analyzing applicant data—such as income, education, and credit scores—the goal is to predict the likelihood of a borrower defaulting on a loan (Binary Classification).

## Task Objective
The primary objective is to develop a robust classification model that can accurately distinguish between approved and rejected loan applications.
**Key Goals:**
1.  Ingest and clean the "Loan Approval Prediction" dataset.
2.  Perform Exploratory Data Analysis (EDA) to understand financial risk factors.
3.  Train a machine learning model (Decision Tree) to classify loan status.
4.  Evaluate performance using Accuracy and Confusion Matrix metrics.

## Approach
The project was implemented in a Jupyter Notebook using Python, following a standard data science pipeline:

1.  **Data Ingestion:**
    * Downloaded the dataset dynamically using `kagglehub`.
    * Loaded the data into Pandas and performed initial inspection.

2.  **Data Cleaning & Preprocessing:**
    * **Formatting:** Cleaned column names by stripping leading/trailing whitespace (e.g., `' education'` → `'education'`).
    * **Sanity Checks:** Verified the absence of missing values to ensure data integrity.
    * **Encoding:** Converted categorical variables (`education`, `self_employed`, `loan_status`) into numerical values (0 and 1) for model compatibility.

3.  **Exploratory Data Analysis (EDA):**
    * **Histograms:** Visualized the distributions of `loan_amount` and `income_annum`.
    * **Count Plots:** Analyzed the relationship between `education` level and loan approval rates.

4.  **Model Training:**
    * Split the data into training (80%) and testing (20%) sets.
    * Implemented a **Decision Tree Classifier** (`max_depth=5`) to capture non-linear decision boundaries in the data.

## Results and Insights
The model was evaluated on the test set with the following findings:

* **Model Accuracy:** The Decision Tree achieved a high accuracy (approximately **97%**), effectively predicting loan outcomes.
* **Key Drivers:** Exploratory analysis and model behavior suggest that the **CIBIL Score** and **Income** are the most dominant factors in determining loan approval.
* **Risk Analysis:** The Confusion Matrix demonstrated the model's ability to minimize False Positives (predicting "Approved" when the actual status was "Rejected"), which is crucial for minimizing financial risk in a real-world lending scenario.
