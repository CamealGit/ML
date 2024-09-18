# Car Price Prediction

## Project Overview

This project involves predicting car prices using a dataset containing various features related to cars. The goal is to estimate car prices based on attributes such as kilometers driven, present price, and fuel type. A Gradient Boosting Regressor is used to build and evaluate the predictive model.


## Steps in the Project

1. **Data Loading:**
   - Loaded the car dataset from a CSV file.

2. **Exploration and Preprocessing:**
   - Analyzed the dataset and performed encoding of categorical variables.
   - Replaced boolean values with integers.
   - Standardized numerical features to ensure uniform scale.

3. **Feature Engineering:**
   - Dropped irrelevant columns that are not needed for the model.
   - Split data into features and target variable.

4. **Model Building:**
   - Used Gradient Boosting Regressor to predict car prices.

5. **Model Evaluation:**
   - Calculated metrics: Mean Absolute Error (MAE), Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R² Score.

## Results

- **MAE (Mean Absolute Error):** 0.09
- **MSE (Mean Squared Error):** 0.02
- **RMSE (Root Mean Squared Error):** 0.15
- **R² Score:** 0.97

## Libraries and Tools

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization.
- **Seaborn**: For statistical data visualization.
- **Scikit-learn**: For machine learning algorithms and metrics, including:
  - **StandardScaler**: For feature scaling.
  - **GradientBoostingRegressor**: For building and training the regression model.
  - **mean_absolute_error**: To calculate MAE.
  - **mean_squared_error**: To calculate MSE.
  - **r2_score**: To calculate R² Score.

