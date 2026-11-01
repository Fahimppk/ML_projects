# 🏦 Bank Loan Prediction – Machine Learning Classification

## 📌 Project Overview

This project focuses on predicting whether a customer will accept a personal loan offer using Machine Learning classification algorithms.

The project involves data loading, data cleaning, exploratory data analysis (EDA), feature preparation, model training, and performance evaluation.

Five different Machine Learning algorithms are implemented and compared to identify the best-performing classification model.

## 🎯 Objectives

- Understand customer data through Exploratory Data Analysis.
- Identify patterns and relationships between customer features.
- Prepare data for Machine Learning.
- Build multiple classification models.
- Compare model performance using evaluation metrics.
- Identify the best-performing model for personal loan prediction.

## 📂 Dataset Information

The dataset contains customer information used to predict personal loan acceptance.

**Target Variable:** `Personal.Loan`

- `0` – Customer did not accept the personal loan.
- `1` – Customer accepted the personal loan.

The target values are converted into `No` and `Yes` for easier interpretation.

### Features used

- Age
- Experience
- Income
- Family
- CCAvg
- Education
- Mortgage
- Securities.Account
- CD.Account
- Online
- CreditCard
- ID

`ZIP.Code` is removed during data preprocessing.

## 🛠️ Technologies & Libraries

- Python
- Jupyter Notebook
- Pandas – Data manipulation
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical visualization
- Scikit-learn – Machine Learning

## 🔍 Exploratory Data Analysis (EDA)

The following EDA operations are performed:

- Data loading and inspection
- Checking dataset shape and structure
- Understanding data types
- Statistical summary using `describe()`
- Missing value detection
- Duplicate value detection
- Target variable analysis
- Box plots
- Count plots
- Line plots
- Correlation analysis
- Correlation heatmap

## ⚙️ Data Preprocessing

- Converted the target variable from numerical values (0 and 1) into categorical labels (`No` and `Yes`).
- Removed the `ZIP.Code` column.
- Separated independent variables (X) and dependent variable (y).
- Split the dataset into training and testing sets.
- Applied StandardScaler for KNN and SVC.

**Train-Test Split:**
- Training data: 80%
- Testing data: 20%
- Random State: 42

## 🤖 Machine Learning Algorithms

Five classification algorithms are implemented:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Support Vector Classifier (SVC)
4. Gaussian Naive Bayes
5. Decision Tree Classifier

## 📊 Model Evaluation

The models are evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report
- Precision
- Recall
- F1-Score

## 🏆 Model Performance Comparison

The following accuracy scores were obtained in the notebook:

| Algorithm | Accuracy |
|---|---:|
| Logistic Regression | 95.20% |
| KNN | 97.10% |
| SVC | 98.50% |
| Gaussian Naive Bayes | 91.60% |
| Decision Tree | **98.70%** |

### Best Performing Model

**Decision Tree Classifier – 98.70% Accuracy**

Among the five implemented algorithms, Decision Tree achieved the highest test accuracy.

SVC also demonstrated strong performance with 98.50% accuracy.

## 📈 Conclusion

This project demonstrates the application of different Machine Learning classification algorithms to a personal loan prediction problem.

By comparing five algorithms, Decision Tree achieved the highest accuracy in the current experiment.

The project also highlights the importance of data preprocessing, feature scaling, exploratory data analysis, and model evaluation in developing Machine Learning solutions.

Further improvements can include Random Forest, hyperparameter tuning, feature selection, and cross-validation.

## 🚀 Future Improvements

- Implement Random Forest Classifier.
- Apply GridSearchCV for hyperparameter tuning.
- Perform cross-validation.
- Remove identifier columns such as ID.
- Compare ROC-AUC and Precision-Recall curves.
- Improve model generalization.

## 👨‍💻 Author

**Muhammed Fahim**

Machine Learning | Data Science | Python.
