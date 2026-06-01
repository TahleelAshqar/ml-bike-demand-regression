# ml-bike-demand-regression
Machine Learning project for predicting bike sharing demand using regression models, feature engineering, hyperparameter tuning, and model comparison.


# Bike Sharing Demand Prediction

This project applies machine learning regression models to predict bike sharing demand based on historical usage and related features.

The notebook includes data preprocessing, exploratory data analysis, feature engineering, model training, hyperparameter tuning, and final model comparison.

## Project Overview

The goal of this project is to predict the number of bike rentals using different regression models and compare their performance using evaluation metrics such as RMSE, MAE, MSE, and R².

## Dataset

The project uses the **Bike Sharing Demand** dataset from OpenML.

The dataset includes features such as:

- Season
- Weather
- Holiday / working day
- Hour
- Month
- Year
- Temperature and other numeric features
- Bike rental count as the target variable

## Models Used

The following regression models were trained and evaluated:

- Random Forest Regressor
- Gradient Boosting Regressor
- Ridge Regression
- SGD Regressor
- Ridge Regression with Polynomial Features
- SGD Regressor with Polynomial Features
- Neural Network using MLPRegressor

## Main Steps

1. Load the Bike Sharing Demand dataset
2. Remove leaky columns such as `casual`, `registered`, and `datetime.`
3. Prepare categorical and numeric features
4. Perform exploratory data visualization
5. Train several regression models
6. Tune hyperparameters using `RandomizedSearchCV.`
7. Apply polynomial feature engineering
8. Compare all models using test performance metrics
9. Select the best model based on Test RMSE

## Evaluation Metrics
The models are compared using:

- Mean Squared Error — MSE
- Root Mean Squared Error — RMSE
- Mean Absolute Error — MAE
- R² Score

The final model selection is based mainly on **Test RMSE**, since the hyperparameter search was optimized using negative root mean squared error.

## Technologies Used
- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- OpenML
- Jupyter Notebook

## How to Run
1. Clone the repository:

```bash
git clone https://github.com/your-username/bike-sharing-demand-prediction.git
