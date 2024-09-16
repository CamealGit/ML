# Diamonds Price Prediction

## Project Overview

This project involves predicting diamond prices using the `diamonds` dataset. The goal is to estimate diamond prices based on various features such as carat, cut, color, and clarity. I used a Random Forest algorithm to build and evaluate the predictive model.

## Project Structure

- `diamonds.ipynb` - Jupyter Notebook containing the full data analysis, including preprocessing, model training, and evaluation.

## Steps in the Project

1. **Data Loading:**
   - Loaded the diamond dataset from a CSV file.

2. **Exploration and Preprocessing:**
   - Analyzed correlations between features and diamond price.
   - Dropped irrelevant columns and encoded categorical variables.

3. **Standardization:**
   - Standardized numerical features to ensure uniform scale.

4. **Model Building:**
   - Used Random Forest Regressor to predict diamond prices.

5. **Model Evaluation:**
   - Calculated metrics: MSE, RMSE, R² Score.

## Results

- **MSE (Mean Squared Error):** 287,021.19
- **RMSE (Root Mean Squared Error):** 535.74
- **R² Score:** 0.98

The model achieved a very good R² Score, indicating high prediction accuracy.

## Libraries and Tools

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization.
- **Seaborn**: For statistical data visualization.
- **Scikit-learn**: For machine learning algorithms and metrics, including:
  - **StandardScaler**: For feature scaling.
  - **RandomForestRegressor**: For building and training the regression model.
  - **mean_squared_error**: To calculate MSE.
  - **r2_score**: To calculate R² Score.
