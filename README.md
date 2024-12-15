# Salary Prediction Using Ordinal Logistic Regression 📊💼

## Overview 🌟
This project tackles the real-world challenge of **predicting annual compensation buckets** for data science professionals using survey data from the **2022 Kaggle Machine Learning & Data Science Survey**. With a focus on **ordinal classification**, the study delves into feature engineering, model tuning, and performance evaluation to uncover key factors influencing salaries in the tech industry.

---

## Problem Statement 🧩
Understanding salary dynamics is crucial for aspiring and current data scientists to navigate their career paths effectively. While traditional regression models predict absolute values, they fail to account for the ordinal nature of salary brackets. This project addresses:

1. **How can ordinal logistic regression predict salary buckets effectively?**
2. **What survey features significantly influence annual compensation?**
3. **How do hyperparameters and feature selection enhance the predictive performance of the model?**

---

## Approach 🚀
This project implements a systematic, data-driven approach:

1. **Data Cleaning & Preprocessing**:
   - Dropped irrelevant features and handled missing values logically.
   - Transformed categorical features into meaningful numeric encodings.
   - Enhanced interpretability with feature engineering, e.g., `Country_Salary_Rank`.

2. **Exploratory Data Analysis (EDA)**:
   - Ranked and visualized features using `SelectKBest` and mutual information regression.
   - Generated new insights, such as grouping job titles and countries by tech salary indices.

3. **Model Development**:
   - Implemented **Ordinal Logistic Regression** for multi-class classification.
   - Applied **10-fold cross-validation** to evaluate model stability and accuracy.

4. **Hyperparameter Tuning**:
   - Optimized regularization (`C`) and penalty types (`L1` vs. `L2`) for bias-variance trade-offs.
   - Evaluated models using **Mean Absolute Error (MAE)** for better misclassification interpretation.

5. **Insights & Testing**:
   - Analyzed prediction distribution trends to detect underfitting and imbalanced data challenges.
   - Highlighted key drivers like **Years of Experience** and **Country Salary Rank**.

---

## Results 🎯
- **Training Accuracy**: 40.2%
- **Testing Accuracy**: 41.4%
- **Key Insights**:
  - Salary disparities are heavily influenced by geographical location and professional experience.
  - Despite reasonable accuracy, the model showed limitations in capturing high salary ranges due to dataset imbalance and model simplicity.

---

## Technologies Used 🛠️
- **Python 3.x**: Core programming language.
- **Libraries**: 
  - `sklearn` for feature selection, modeling, and evaluation.
  - `pandas` & `numpy` for data handling and preprocessing.
  - `matplotlib` & `seaborn` for visualizations.
- **Jupyter Notebook**: Interactive development environment.
- **Google Colab**: Cloud-based execution platform.

---

## Key Features ✨

- **Feature Engineering**: Explored new ways to extract and encode information, such as country rank and job importance scores, to improve interpretability and prediction accuracy.
- **Ordinal Regression Focus**: Implemented ordinal logistic regression to effectively account for the natural order of salary buckets, enhancing the model's relevance for the task.
- **Bias-Variance Trade-off**: Conducted a detailed analysis of hyperparameters like regularization strength (`C`) to balance bias and variance, optimizing model performance.

---

## Next Steps 🧭

- **Address Dataset Imbalance**: Incorporate advanced sampling techniques to mitigate the impact of imbalanced salary buckets on model training.
- **Experiment with Complex Models**: Explore advanced algorithms such as Gradient Boosting Machines (e.g., XGBoost) for better predictive performance.
- **Explore Other Ordinal Algorithms**: Investigate additional methods tailored to ordinal data for improved prediction in higher salary brackets.

---

Feel free to **clone**, **explore**, and **experiment** with the project! Contributions are welcome to take this analysis further. 🚀✨
---

## Repository Structure 📂
```plaintext
├── clean_kaggle_data_2022.csv     # Cleaned dataset used for the assignment
├── salary_prediction.ipynb  # Jupyter Notebook with detailed implementation
├── README.md                    # This file: Detailed project overview



