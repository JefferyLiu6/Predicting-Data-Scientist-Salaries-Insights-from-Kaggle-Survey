# Predicting Data Scientist Salaries: An Ordinal Classification Approach

## Problem Statement
Understanding what drives salary variations in the data science field is a pressing challenge for job seekers, educators, and employers alike. With diverse factors such as geography, experience, and education contributing to compensation, there is a need for a systematic analysis of survey data to uncover patterns and predict salary buckets effectively.

## Project Overview
This project utilizes the Kaggle 2022 Machine Learning & Data Science Survey dataset to explore and address the following question:

**How can survey data from the global data science community be leveraged to predict a respondent's yearly compensation bucket accurately?**

To answer this, I implemented a pipeline for data preprocessing, feature engineering, and model development. The project focuses on using ordinal logistic regression for multi-class classification, supported by exploratory data analysis, feature selection, and hyperparameter tuning.

---

## Key Highlights

### 1. Data Cleaning and Preprocessing
- Handled missing data using appropriate imputation strategies to preserve dataset integrity.
- Encoded categorical variables (e.g., countries, job titles) using label encoding and ordinal mapping to maintain logical order.
- Standardized numerical features to improve model performance and ensured compatibility with logistic regression.

### 2. Exploratory Data Analysis and Feature Engineering
- Conducted feature importance analysis to identify key predictors of salary, such as geography, experience, and education.
- Created new features (e.g., salary rank by country and job title) to capture nuanced relationships.
- Reduced dimensionality using feature selection techniques to improve model interpretability.

### 3. Model Development and Evaluation
- Implemented ordinal logistic regression with a focus on balancing bias and variance through hyperparameter tuning.
- Performed 10-fold cross-validation to evaluate model consistency and robustness.
- Selected the best-performing model using mean absolute error (MAE) as a metric, emphasizing the importance of reducing severe misclassifications in ordinal classification.

### 4. Visualization and Insights
- Visualized feature importance and data distributions to communicate findings effectively.
- Analyzed model predictions against true salary buckets to identify underfitting and imbalanced data issues.

---

## Results and Takeaways

- **Accuracy**: The tuned ordinal logistic regression model achieved an average accuracy of ~40% on the test set, significantly better than random guessing (1/15 for 15 classes).
- **Key Predictors**: Features like `Country_Salary_Rank` and `Years of Coding Experience` emerged as top predictors, highlighting the influence of geography and professional experience on salary.
- **Model Limitations**: The model underperformed in higher salary categories due to data imbalance, pointing to the need for more comprehensive datasets and advanced techniques.

---

## Tools and Technologies
- **Libraries**: NumPy, Pandas, Scikit-learn, Matplotlib, Seaborn
- **Platform**: Google Colab

---

## Repository Contents
- **Notebook**: `lastname_studentnumber_assignment2.ipynb` – Contains the full implementation, including data preprocessing, feature engineering, and model development.
- **Report**: `lastname_studentnumber_assignment2.pdf` – A concise report summarizing methodology, results, and insights.
- **Dataset**: `clean_kaggle_data_2022.csv` – The processed dataset used for this assignment.

---

## Applications
This project provides a framework for:
- Building predictive models for ordinal classification tasks in various domains.
- Identifying key factors influencing outcomes in multi-dimensional survey data.
- Developing transparent and interpretable machine learning pipelines for real-world applications.
