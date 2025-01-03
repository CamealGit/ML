# Breast Calories Prediction with XGBoost

## Project Overview

This project aims to predict the number of calories burned during exercise based on various features such as age, height, weight, duration, and heart rate. We use the XGBoost regression model to build the prediction model and evaluate its performance.

## Dataset

- **Source**: The dataset consists of two CSV files: `calories.csv` and `exercise.csv`.
- **Features**: Includes attributes like age, height, weight, exercise duration, heart rate, and gender.
- **Target**: The target variable is the number of calories burned (`Calories`).

## Steps

1. **Data Loading**: The data is loaded from CSV files using `pandas`.
2. **Data Exploration**: We perform basic data exploration and calculate summary statistics.
3. **Correlation Analysis**: Visualized the correlation matrix to understand relationships between numeric features.
4. **Data Preprocessing**:
    - Converted gender to numeric values (0 for male, 1 for female).
    - Standardized numeric columns (`Age`, `Height`, `Weight`, `Duration`, `Heart_Rate`).
5. **Model Building**:
    - Built a regression model using `XGBRegressor` from XGBoost.
6. **Model Training**: Trained the model using the training data.
7. **Model Evaluation**:
    - Evaluated the model performance using four key evaluation metrics:
        - **Mean Absolute Error (MAE)**
        - **Mean Squared Error (MSE)**
        - **Root Mean Squared Error (RMSE)**
        - **R² Score**
8. **Results**: Displayed the evaluation metrics to assess the model's prediction accuracy.

## Evaluation Metrics

The following metrics were used to evaluate the model's performance:

- **Mean Absolute Error (MAE)**: 1.48
- **Mean Squared Error (MSE)**: 4.71
- **Root Mean Squared Error (RMSE)**: 2.17
- **R² Score**: 1.00
    - The model explains **100%** of the variance in the test data, indicating an ideal fit.

## Conclusion

The model demonstrates excellent performance, with a **1.00 R² score**, indicating that it can predict the number of calories burned with near-perfect accuracy. The MAE, MSE, and RMSE also suggest that the model makes minimal errors in its predictions. This showcases the power of XGBoost for regression tasks in predicting numerical outcomes.

---

Libraries Used:

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations and array handling.
- **Matplotlib & Seaborn**: For data visualization.
- **Scikit-learn**: For model evaluation and data preprocessing.
- **XGBoost**: For building and training the regression model.
