# 🏠 House Price Prediction using Machine Learning

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange?logo=scikitlearn)
![XGBoost](https://img.shields.io/badge/XGBoost-Regression-green)
![License](https://img.shields.io/badge/License-MIT-yellow)
![Kaggle](https://img.shields.io/badge/Kaggle-House%20Prices-blue?logo=kaggle)

---

## 📖 Project Overview

This project presents a complete end-to-end **Machine Learning Regression** workflow for predicting residential house prices using the **House Prices: Advanced Regression Techniques** dataset provided by Kaggle.

The objective is to develop an accurate regression model capable of estimating house selling prices based on various structural, environmental, and neighborhood characteristics.

The project follows a standard Data Science pipeline, including data exploration, preprocessing, feature engineering, model development, evaluation, hyperparameter optimization, and final prediction generation.

---

## 🎯 Business Objective

House prices are influenced by many factors such as property size, construction quality, neighborhood, garage capacity, and renovation history.

The objective of this project is to build a regression model that minimizes prediction error while providing accurate and reliable estimates of residential property prices.

---

## 🤖 Machine Learning Objective

Three regression algorithms were implemented and compared:

- Linear Regression
- Random Forest Regressor
- Extreme Gradient Boosting (XGBoost)

The final model was selected based on the lowest **Root Mean Squared Error (RMSE)**.

---

# 📂 Dataset

Dataset Source:

**Kaggle - House Prices: Advanced Regression Techniques**

https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques

Dataset contains:

- train.csv
- test.csv
- sample_submission.csv
- data_description.txt

---

# 🛠 Technologies Used

Programming Language

- Python

Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost
- Joblib

Environment

- Google Colab
- Kaggle

---

# 📊 Project Workflow

```
Business Understanding
        │
        ▼
Data Understanding
        │
        ▼
Exploratory Data Analysis (EDA)
        │
        ▼
Data Cleaning
        │
        ▼
Feature Engineering
        │
        ▼
Missing Value Imputation
        │
        ▼
One-Hot Encoding
        │
        ▼
ColumnTransformer Pipeline
        │
        ▼
Train-Test Split
        │
        ▼
Model Training
        │
        ▼
Cross Validation
        │
        ▼
Hyperparameter Tuning
        │
        ▼
Model Evaluation
        │
        ▼
Feature Importance
        │
        ▼
Prediction
        │
        ▼
submission.csv
```

---

# 📈 Exploratory Data Analysis (EDA)

The following analyses were performed:

- Distribution of SalePrice
- Log Transformation of SalePrice
- Numerical Feature Distribution
- Missing Value Analysis
- Correlation Analysis
- Correlation Heatmap
- Top Features Correlated with SalePrice
- Outlier Detection
- OverallQual vs SalePrice
- GrLivArea vs SalePrice
- GarageCars vs SalePrice
- YearBuilt vs SalePrice
- Neighborhood Analysis
- Pairplot of Important Features

---

# ⚙ Data Preprocessing

The preprocessing stage includes:

## Missing Value Handling

- Median Imputation for Numerical Features
- Most Frequent Imputation for Categorical Features

---

## Feature Engineering

Several new features were created:

- TotalSF
- HouseAge
- RemodelAge
- TotalBathrooms
- TotalPorchSF
- HasGarage
- HasBasement

---

## Feature Encoding

Categorical variables were encoded using

- One-Hot Encoding

---

## Pipeline

A complete preprocessing pipeline was implemented using

- ColumnTransformer
- Pipeline

This approach ensures reproducible preprocessing and prevents data leakage.

---

# 🧠 Machine Learning Models

The following regression algorithms were evaluated:

| Model | Description |
|--------|-------------|
| Linear Regression | Baseline Regression Model |
| Random Forest Regressor | Ensemble Learning |
| XGBoost Regressor | Gradient Boosting |

---

# 🔍 Cross Validation

5-Fold Cross Validation was applied to estimate the generalization capability of each regression model.

---

# 🎯 Hyperparameter Tuning

RandomizedSearchCV was used to optimize

Random Forest

- Number of Trees
- Maximum Depth
- Minimum Samples Split
- Minimum Samples Leaf

XGBoost

- Learning Rate
- Maximum Depth
- Number of Estimators
- Subsample
- Column Sample By Tree

---

# 📏 Evaluation Metrics

The regression models were evaluated using

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

The best-performing model was selected based on the lowest RMSE.

---

# 📊 Model Interpretation

Model interpretation includes

- Feature Importance
- Actual vs Predicted Plot
- Residual Analysis

These analyses help explain model behavior and identify prediction errors.

---

# 📁 Repository Structure

```
House-Price-Prediction/

│

├── data/

│   ├── train.csv

│   ├── test.csv

│   ├── sample_submission.csv

│

├── notebook/

│   └── House_Price_Prediction.ipynb

│

├── output/

│   └── submission.csv

│

├── model/

│   └── house_price_model.pkl

│

├── images/

│   ├── saleprice_distribution.png

│   ├── heatmap.png

│   ├── feature_importance.png

│   ├── residual_plot.png

│   └── actual_vs_prediction.png

│

├── README.md

├── requirements.txt

├── LICENSE

└── .gitignore
```

---

# 🚀 Running the Project

## Clone Repository

```bash
git clone https://github.com/yourusername/House-Price-Prediction.git
```

```bash
cd House-Price-Prediction
```

---

Install dependencies

```bash
pip install -r requirements.txt
```

---

Run Jupyter Notebook

```bash
jupyter notebook
```

or open directly using

Google Colab

---

# 📦 Output

The notebook automatically generates

```
submission.csv
```

The file follows the Kaggle submission format

| Id | SalePrice |
|----|----------:|
|1461|169277.05|
|1462|187583.22|
|...|...|

---

The trained model is also saved as

```
house_price_model.pkl
```

which can be used for future inference or deployment.

---

# 📈 Future Improvements

Possible future enhancements include

- LightGBM
- CatBoost
- Stacking Ensemble
- Bayesian Hyperparameter Optimization
- SHAP Explainability
- Model Deployment using Streamlit
- Docker Containerization

---

# 📚 References

1. Kaggle - House Prices: Advanced Regression Techniques

https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques

2. Scikit-Learn Documentation

https://scikit-learn.org/

3. XGBoost Documentation

https://xgboost.readthedocs.io/

---

# 👨‍💻 Author

**Tegar Reski Pratama**

Department of Informatics

Faculty of Engineering

Universitas Muhammadiyah Malang

GitHub:
[https://github.com/yourusername](https://github.com/TegarReskiPratama)

LinkedIn:
https://www.linkedin.com/in/tegar-reski-pratama-47491822a/

---

# ⭐ Support

If you find this project useful, consider giving this repository a ⭐ on GitHub.

Thank you for visiting!
