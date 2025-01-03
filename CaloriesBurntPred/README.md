# Calories Burnt Prediction with XGBoost

## Project Overview

This project involves predicting the number of calories burnt during exercise based on various features using the XGBoost regression model. The dataset includes demographic and physiological data related to exercise sessions.

## Dataset

- **Source**: Two CSV files:
    - `calories.csv`: Contains the target variable (Calories).
    - `exercise.csv`: Contains demographic and physiological features.
- **Features**:
    - Demographic: Gender, Age, Height, Weight.
    - Physiological: Duration of exercise, Heart rate.
- **Target**: Calories burnt during exercise.

## Steps

1. **Data Loading**:
    - Loaded the datasets using `pandas`.
    - Merged the `exercise` dataset with the `Calories` column.
2. **Data Exploration**:
    - Examined descriptive statistics for all features using `describe()`.
    - Visualized feature correlations using a heatmap.
3. **Data Preprocessing**:
    - Converted `Gender` to numerical values (0 for male, 1 for female).
    - Dropped unnecessary columns like `User_ID`.
    - Standardized numerical features (`Age`, `Height`, `Weight`, `Duration`, `Heart_Rate`) using `StandardScaler`.
4. **Data Splitting**:
    - Split the dataset into training and testing sets (80/20 split).
5. **Model Building and Training**:
    - Utilized the `XGBRegressor` model to fit the training data.
6. **Prediction and Evaluation**:
    - Made predictions on the test set.
    - Evaluated the model using Mean Absolute Error (MAE).

## Results

- **MAE**: The model achieved a mean absolute error of **{insert MAE value}**, indicating its performance in predicting calories burnt.

## Conclusion

The XGBoost model demonstrated the ability to predict the number of calories burnt during exercise with reasonable accuracy. Further optimization and feature engineering may improve the model's performance.

---

## Libraries Used

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib & Seaborn**: For data visualization.
- **Scikit-learn**: For data preprocessing, splitting, and evaluation.
- **XGBoost**: For building the regression model.
