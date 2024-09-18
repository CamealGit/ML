# Gold Price Prediction with Random Forest Regressor

## Project Overview

This project aims to predict gold prices using a Random Forest Regressor. The dataset used contains historical gold price data, and the goal is to build and evaluate a model to forecast future gold prices based on historical features.

## Dataset

- **Source**: `gld_price_data.csv`
- **Features**: Various numerical features related to gold prices.
- **Target**: Gold prices (`GLD`).

## Steps

1. **Data Loading**:
   - Loaded the gold price dataset from a CSV file.

2. **Data Exploration**:
   - Displayed basic information and summary statistics of the dataset.
   - Dropped the 'Date' column for correlation analysis.

3. **Correlation Analysis**:
   - Calculated and visualized the correlation matrix of features with the target variable (`GLD`).
   - Plotted the distribution of the target variable (`GLD`).

4. **Data Preparation**:
   - Separated features (`X`) and the target variable (`Y`).
   - Split the dataset into training and testing sets (80% train, 20% test).

5. **Model Training**:
   - Initialized and trained a Random Forest Regressor with 100 estimators.

6. **Model Evaluation**:
   - Predicted the target variable for the test set.
   - Calculated the R-squared score to evaluate model performance.

## Results

- **R-squared Score**: The R-squared score on the test set is 0.99

## Conclusion

The Random Forest Regressor model has been trained and evaluated on gold price data, providing an R-squared score that reflects the model's performance in predicting gold prices.

## Libraries Used

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization.
- **Seaborn**: For statistical data visualization.
- **Scikit-learn**: For machine learning algorithms and metrics, including:
  - **RandomForestRegressor**: For building and training the regression model.
  - **metrics.r2_score**: To calculate the R-squared score.
