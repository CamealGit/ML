# Big Mart Sales Prediction with XGBoost

## Project Overview

This project focuses on predicting sales for Big Mart items using the XGBoost Random Forest Regressor. The dataset used, `Train.csv`, contains various features related to items and their outlets. The objective is to build and evaluate a model to accurately predict item outlet sales.

## Dataset

- **Source**: Big Mart Sales dataset (`Train.csv`).
- **Features**: Various features including item weight, item fat content, item type, outlet identifier, and outlet size.
- **Target**: Continuous variable representing item outlet sales.

## Steps

1. **Data Loading**: Loaded the dataset from a CSV file into a pandas DataFrame.
2. **Data Cleaning**:
   - Checked for and handled missing values:
     - Filled missing `Item_Weight` with the mean value.
     - Filled missing `Outlet_Size` based on the mode for each `Outlet_Type`.
   - Replaced inconsistent categories in `Item_Fat_Content` with standardized labels.
3. **Data Encoding**:
   - Encoded categorical variables into numerical labels using `LabelEncoder`.
4. **Feature and Target Separation**:
   - Separated the features (independent variables) and target (sales).
5. **Data Splitting**:
   - Split the dataset into training and testing sets.
6. **Model Building**:
   - Initialized and trained an `XGBRFRegressor` model from the XGBoost library.
7. **Model Evaluation**: 
   - Predicted sales on training and test data.
   - Calculated and printed the R² score for both training and test data to evaluate model performance.

## Results

- **Training R² Score**: Achieved a score of `r2_train` (value will be printed during execution).
- **Test R² Score**: Achieved a score of `r2_test` (value will be printed during execution).

## Conclusion

The XGBoost Random Forest Regressor provides a robust model for predicting item outlet sales based on the features provided. The model's performance, as indicated by the R² scores, demonstrates its effectiveness in making accurate predictions.

## Libraries Used

- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical operations.
- **Scikit-learn**: For train-test splitting and metrics.
- **XGBoost**: For the Random Forest Regressor model.
- **Matplotlib & Seaborn**: For visualization.

