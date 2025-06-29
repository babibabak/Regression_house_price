# Regression_house_price
A machine learning project for predicting house prices using a dataset with features like area, number of rooms, and parking availability. The project implements Linear Regression, Polynomial Regression, and Support Vector Regression (SVR) models, with data preprocessing
## Overview

This project aims to predict house prices using a dataset containing features such as area, number of rooms, parking, warehouse, elevator, and address. The project involves data preprocessing, exploratory data analysis (EDA), and the application of multiple machine learning models, including Linear Regression, Polynomial Regression, and Support Vector Regression (SVR). The models are evaluated using Mean Squared Error (MSE) and R² score to assess prediction accuracy.

## Features
- Data Preprocessing: Converting boolean features (Parking, Warehouse, Elevator) to integers, handling non-numeric values in the Area column, and selecting relevant features for modeling.

- Exploratory Data Analysis (EDA): Visualizing relationships between features and house prices (in USD) using          scatter plots and correlation analysis.

- Machine Learning Models:
    - Linear Regression for baseline prediction.
    - Polynomial Regression to capture non-linear relationships.
    - Support Vector Regression (SVR) for robust regression modeling.

- Model Evaluation: Assessing model performance using MSE and R² score, with Linear Regression achieving an R² score of 0.51 on the test set.

- Data Splitting: Randomly splitting data into 80% training and 20% testing sets.

## Dataset

The dataset (house_price.csv) contains 3,473 house records with the following features:
- Area (integer), Room (integer), Parking (binary), Warehouse (binary), Elevator (binary), Address (string), Price (in local currency), Price(USD) (target variable).

## Requirements
- Python 3.11
- Libraries: `numpy`, `pandas`, `scikit-learn`, `matplotlib`, `seaborn`

## Installation

1.Clone the repository:
```bash
    git clone https://github.com/yourusername/house-price-prediction.git
```
2.Install dependencies:
```bash
    pip install -r requirements.txt
```
3.Run the Jupyter Notebook:
```bash
    jupyter notebook house_price.ipynb
```
## Usage
- Load and preprocess the dataset (convert data types, handle missing values).
- Perform EDA to explore feature correlations and visualize data distributions.
- Train and evaluate Linear Regression, Polynomial Regression, and SVR models.
- Assess model performance using MSE and R² score.

## Model Performance
- Linear Regression:
    - Residual Sum of Squares (MSE): 35,173,825,859.18
    - R² Score: 0.51
- Polynomial Regression and SVR: Implemented for comparison (specific metrics not fully detailed in the notebook).

## Future Improvements
- Perform hyperparameter tuning for SVR and Polynomial Regression.
- Incorporate additional features (e.g., Address) via encoding techniques.
- Experiment with advanced models like Random Forest or Gradient Boosting.
- Enhance EDA with more visualizations to uncover deeper insights.
