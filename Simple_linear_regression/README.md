# Salary Prediction – Exploratory Data Analysis and Linear Regression

## Project Overview

This beginner-friendly project explores a salary dataset and uses **Linear Regression** to study the relationship between years of work experience and salary.

The notebook contains simple Exploratory Data Analysis (EDA) steps followed by a Linear Regression workflow.

## Dataset

The notebook expects a CSV file named:

```text
Salary_Data.csv
```

The dataset should contain these columns:

- `YearsExperience` – years of work experience
- `Salary` – salary value

Place `Salary_Data.csv` in the same folder as the Jupyter Notebook.

## EDA Steps

The notebook covers:

1. Display the first rows using `head()`
2. Check the dataset size using `shape`
3. Check column information using `info()`
4. View statistics using `describe()`
5. Check missing values using `isnull().sum()`
6. Check duplicate rows using `duplicated().sum()`
7. Check data types using `dtypes`
8. Plot histograms to understand distributions
9. Use boxplots to inspect possible outliers
10. Use a scatter plot to compare experience and salary
11. Use a regression plot to view the linear relationship
12. Check correlation using `corr()`
13. Display a correlation heatmap

The EDA code is written in a simple, beginner-friendly style. It avoids `if`, `else`, and `for` loops.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn (for Linear Regression)

## Installation

Install the required libraries:

```bash
pip install pandas matplotlib seaborn scikit-learn jupyter
```

## How to Run

1. Download or clone this project.
2. Keep `Salary_Data.csv` and the notebook in the same folder.
3. Open a terminal in the project folder.
4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open `linear_regression_simple_eda.ipynb`.
6. Run the notebook cells from top to bottom.

## Project Structure

```text
salary-prediction/
│
├── linear_regression_simple_eda.ipynb
├── Salary_Data.csv
└── README.md
```

## Learning Outcomes

After completing this project, you will understand:

- How to load and inspect a dataset
- How to identify missing and duplicate values
- How to explore numerical data with plots
- How to understand correlation
- How to examine the relationship between two variables
- How EDA supports a Linear Regression task

## Note

This is a learning project. The notebook assumes the dataset has the column names `YearsExperience` and `Salary`. If your CSV uses different names, update the column references in the notebook.
