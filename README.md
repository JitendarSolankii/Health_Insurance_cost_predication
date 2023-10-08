# Health_Insurance_cost_predication
### Health Insurance Cost Prediction Project
## Overview
This project aims to predict the best price for health insurance using machine learning models. The dataset used for this project includes features such as age, gender, BMI, number of children, smoking status, location, and health insurance price.

## Steps
## 1. Data Loading and Initial Exploration
The dataset is loaded using pandas from an Excel file (Health_insurance_cost.xlsx).
Initial exploration is performed using functions like mean(), info(), and describe().
Column names are standardized and missing values are identified.

## 2. Handling Missing Values
Missing values in the 'age', 'BMI', and 'insurance_price' columns are imputed with the mean values.
The dataset is checked to ensure no missing values remain.

## 3. Exploratory Data Analysis (EDA)
Visualizations are created to explore the distribution of health insurance prices and relationships between variables.
Histograms, scatter plots, and box plots are used to gain insights.

## 4. Data Preprocessing
Label encoding is applied to convert categorical variables ('sex', 'smoker', 'location') into numerical format.
Standard scaling is performed on numerical features ('age', 'BMI', 'Children').

## 5. Model Training and Evaluation
The dataset is split into training and testing sets.
Linear Regression, Decision Tree Regression, Random Forest Regression, and XGBoost Regression models are trained and evaluated using mean squared error (MSE) and mean absolute error (MAE).

## 6. Compare Model Performance
Model performance metrics (MSE and MAE) are compared to identify the best-performing model.

## 7. Determine the Best Model
The model with the lowest MSE is considered the best for predicting health insurance costs.
The selected best model is XGBRegressor.

How to Use
Install the required libraries:

bash
Copy code
pip install pandas numpy matplotlib seaborn plotly openpyxl missingno scikit-learn xgboost
Run the Jupyter notebook or Python script.

Explore the visualizations and evaluation metrics.

Adjust the models or hyperparameters as needed.

Results
Model Performance
Linear Regression MSE: 34,651,854.36, MAE: 4,222.08
Decision Tree Regression MSE: 43,120,500.59, MAE: 3,092.80
Random Forest Regression MSE: 22,322,803.77, MAE: 2,600.37
XGBRegressor MSE: 26,182,081.32, MAE: 2,792.78
Best Model
The best model for predicting health insurance costs is XGBRegressor.

## Conclusion
This project demonstrates the process of predicting health insurance costs, from data loading and exploration to model training and evaluation. The selected XGBRegressor model provides the most accurate predictions based on MSE and MAE metrics.



