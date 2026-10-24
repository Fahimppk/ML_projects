# 🚗 Car Price Prediction using Machine Learning

## 📌 Project Overview

This project uses Machine Learning to predict the price of a used Ford car based on its features. It applies Exploratory Data Analysis (EDA), data preprocessing, feature engineering, and Linear Regression to understand the factors associated with car prices and generate predictions.

The project uses Python and Scikit-learn to build and evaluate a regression model.

## 🎯 Objectives

- Explore and understand the used-car dataset.
- Identify relationships between car features and prices.
- Clean duplicate records and prepare data for machine learning.
- Engineer a new feature representing car age.
- Train a Linear Regression model.
- Evaluate model performance using regression metrics.

## 📊 Dataset

**Dataset:** Ford car prices (`ford.csv`)

The dataset includes features such as:

| Feature | Description |
|---|---|
| `model` | Ford car model |
| `year` | Year of manufacture |
| `price` | Car selling price (target variable) |
| `transmission` | Transmission type |
| `mileage` | Distance travelled |
| `fuelType` | Type of fuel |
| `tax` | Vehicle tax |
| `mpg` | Miles per gallon |
| `engineSize` | Engine size |

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## 🔍 Project Workflow

### 1. Data Loading and Inspection
- Loaded the Ford car dataset using Pandas.
- Inspected the dataset using `head()`, `describe()`, and `shape`.
- Checked missing values and duplicate records.

### 2. Exploratory Data Analysis (EDA)
- Visualized the distribution of car prices.
- Analyzed correlations between numerical features.
- Explored the relationship between price and year, mileage, engine size, tax, and transmission.
- Used histograms, boxplots, line plots, and a correlation heatmap.

### 3. Data Preprocessing
- Removed duplicate records.
- Excluded records with a year of manufacture greater than or equal to 2026.
- Created a `car_age` feature from the year of manufacture.
- Removed the original `year` and target `price` columns from the input features.

### 4. Feature Engineering and Encoding
- Applied one-hot encoding to `model`, `transmission`, and `fuelType`.
- Standardized the numerical features `mileage`, `tax`, `mpg`, `car_age`, and `engineSize`.

### 5. Model Training
- Split the dataset into training and testing sets.
- Used an 80:20 train-test split with `random_state=30`.
- Trained a Linear Regression model using Scikit-learn.

### 6. Model Evaluation
Evaluated the model using:

- **R² Score:** Measures the proportion of variance in car prices explained by the model.
- **Mean Squared Error (MSE):** Measures the average squared prediction error.
- **Root Mean Squared Error (RMSE):** Measures prediction error in the target's units.

## 📈 Model Performance

The notebook calculates R², MSE, and RMSE after making predictions on the test set. Run the notebook to obtain the actual evaluation results.

| Metric | Purpose |
|---|---|
| R² Score | Measures goodness of fit |
| MSE | Measures squared prediction error |
| RMSE | Measures error in price units |

## 📂 Repository Structure

```text
Car-Price-Prediction/
├── code/
│   └── CarPricePredictionModel.ipynb
├── output_images/
│   ├── price_distribution.png
│   ├── correlation_heatmap.png
│   ├── price_vs_year.png
│   ├── price_vs_mileage.png
│   └── price_vs_engine_size.png
├── README.md
└── requirements.txt
```

*The image filenames above are suggested examples; add them after exporting the actual charts from your notebook.*

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
cd Car-Price-Prediction
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Prepare the dataset

Download or obtain `ford.csv` and place it in the location expected by the notebook. For easier portability, consider storing the dataset in a `data/` folder and loading it with a relative path.

### 4. Run the notebook

```bash
jupyter notebook
```

Open `code/CarPricePredictionModel.ipynb` and execute the cells.

## 💡 Key Learning Outcomes

- Performing EDA on a real-world dataset.
- Cleaning and preprocessing data.
- Encoding categorical variables.
- Feature engineering.
- Applying feature scaling.
- Training a regression model.
- Evaluating predictions using regression metrics.

## 🔮 Future Improvements

- Compare Linear Regression with Random Forest and other regression algorithms.
- Use cross-validation and hyperparameter tuning.
- Improve preprocessing by fitting transformations only on training data using a Scikit-learn pipeline.
- Investigate influential features and prediction errors.
- Build a simple web application for interactive car price predictions.

## 👨‍💻 About

This project is part of my hands-on learning journey in **Data Science, Artificial Intelligence, and Machine Learning**. It demonstrates the application of Python-based data analysis and regression techniques to a real-world price prediction problem.

---

⭐ If you find this project useful, feel free to explore the code and share feedback.
