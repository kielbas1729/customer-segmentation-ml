# Automobile Customer Segmentation Classification

## Project Overview
[cite_start]The primary objective of this project is to develop and evaluate machine learning models for the classification of automobile customers into four pre-defined segments: A, B, C, and D[cite: 9]. [cite_start]By analyzing demographic and behavioral data, the project compares the performance of several classification algorithms to identify the most effective solution for targeted marketing strategies[cite: 9, 772].

## Dataset
[cite_start]The data is sourced from Kaggle's "Customer Segmentation" dataset[cite: 10]. [cite_start]It includes 10,695 records with the following features[cite: 42, 43]:
* [cite_start]**Demographics:** Gender, Age, Ever Married, Graduated[cite: 47, 50, 54, 58, 62].
* [cite_start]**Employment:** Profession, Work Experience[cite: 66, 70].
* [cite_start]**Lifestyle:** Spending Score, Family Size[cite: 74, 78].
* [cite_start]**Target Variable:** Segmentation (Groups A, B, C, D)[cite: 84].

## Technical Implementation
[cite_start]The project was conducted in a Google Colab environment using Python and industry-standard libraries[cite: 1, 11]:
* [cite_start]**Data Processing:** Pandas, NumPy[cite: 14, 15].
* [cite_start]**Feature Engineering:** OneHotEncoder for categorical variables and StandardScaler for feature scaling[cite: 18, 421].
* [cite_start]**Model Selection:** Logistic Regression, K-Nearest Neighbors, Decision Tree, Random Forest, and XGBoost[cite: 21, 22, 23].
* [cite_start]**Optimization:** Hyperparameter tuning was performed using GridSearchCV to find optimal parameters (e.g., max_depth, n_estimators)[cite: 20, 574, 639, 712].

## Performance Results
[cite_start]The models were evaluated based on their accuracy scores on the test set[cite: 415, 773]:

| Model | Test Accuracy |
| :--- | :--- |
| **XGBoost** | **0.487** |
| Random Forest | 0.482 |
| Logistic Regression | 0.477 |
| KNN | 0.469 |
| Decision Tree | 0.464 |

[cite_start][cite: 774, 775, 776, 777, 778]

## Key Conclusions
* [cite_start]**XGBoost** proved to be the most accurate model, successfully capturing complex non-linear patterns in customer behavior, albeit being the most resource-intensive[cite: 813].
* [cite_start]**Logistic Regression** showed surprisingly high effectiveness (0.477 accuracy), suggesting that some underlying relationships between features like age or spending score and the segments are somewhat linear[cite: 814].
* [cite_start]Given the high noise-to-signal ratio inherent in human behavioral data, an accuracy of ~49% for a 4-class problem represents a significant improvement over the baseline random guess of 25%.

## How to Run
1. Clone the repository.
2. Ensure you have `scikit-learn`, `pandas`, `matplotlib`, and `xgboost` installed.
3. The original dataset can be downloaded from [Kaggle](https://www.kaggle.com/datasets/kaushiksuresh147/customer-segmentation/data).
