# Task 1: Exploring and Visualizing a Simple Dataset

## Overview
This project is part of the Data Science & Analytics Internship at DevelopersHub Corporation. The goal of this task is to demonstrate fundamental data science skills, including data ingestion, structural analysis, and exploratory data analysis (EDA) using Python.

## Task Objective
The primary objective is to understand how to read, summarize, and visualize a dataset. Using the classic Iris dataset, the specific goals were to:
1.  Load and inspect the data structure using Pandas.
2.  Verify data integrity (checking for missing values and duplicates).
3.  Create visualizations to analyze relationships, distributions, and outliers using Matplotlib and Seaborn.

## Approach
The analysis was conducted using a Jupyter Notebook/Google Colab environment with the following workflow:

1.  **Data Loading:**
    * Utilized the `pandas` library to load the dataset directly from a raw CSV source.
    * Displayed the first few rows to verify successful ingestion.

2.  **Structure Inspection:**
    * Used `.shape`, `.columns`, and `.info()` to document the dataset's dimensions and data types.

3.  **Data Cleaning:**
    * Performed checks for null values and duplicate entries to ensure data quality before visualization.

4.  **Exploratory Data Analysis (EDA):**
    * **Scatter Plot:** Mapped relationships between Sepal Length and Sepal Width to observe clustering behavior among species.
    * **Histogram:** Analyzed the frequency distribution of Petal Length to identify skewness and modality.
    * **Box Plot:** Examined the spread of Sepal Width across different species to detect outliers and compare variances.

## Results and Insights
Through the visualization and analysis process, the following key insights were derived:

* **Data Quality:** The dataset is highly structured with 150 entries and no missing values, though it contains a small number of duplicate rows.
* **Species Separation:** The *Iris setosa* species is distinct and linearly separable from the other two species (*Versicolor* and *Virginica*) based on sepal dimensions.
* **Feature Distribution:** Petal length exhibits a bimodal distribution, indicating distinct physical characteristics between the species groups.
* **Variance:** *Iris virginica* generally shows a wider variance in features compared to *Iris setosa*, which is more uniform.

These findings suggest that the dataset features, particularly petal dimensions, are strong candidates for training classification models in future steps.
