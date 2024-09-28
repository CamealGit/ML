# Insurance Charges Prediction

This project involves predicting insurance charges based on features such as age, sex, BMI, children, smoker status, and region using machine learning techniques. The model is built using Gradient Boosting Regressor, and its performance is evaluated using metrics like MSE, RMSE, and R² Score.

## Project Overview

The project follows these key steps:
1. **Data Loading**: Load the insurance dataset from a CSV file.
2. **Data Preprocessing**:
   - One-Hot encoding of categorical columns (`sex`, `smoker`, and `region`).
   - Correlation analysis between features and the target (`charges`).
3. **Standardization**: Standardize the features to a uniform scale using `StandardScaler`.
4. **Model Building**: Use a `GradientBoostingRegressor` to predict insurance charges.
5. **Model Evaluation**: Evaluate the model's performance using MSE, RMSE, and R² Score.


## Steps in the Project

### Data Loading
- The insurance dataset (`insurance.csv`) is loaded for analysis and modeling.

### Data Preprocessing
- Performed One-Hot encoding on categorical features (`sex`, `smoker`, `region`).
- Analyzed correlations between features and insurance charges using a heatmap to identify relationships.

### Standardization
- Applied `StandardScaler` to standardize numerical features, ensuring all features are on the same scale.

### Model Building
- A `GradientBoostingRegressor` is used to build a predictive model for insurance charges.

### Model Evaluation
- The model's performance is evaluated using the following metrics:
  - **MSE (Mean Squared Error)**: Quantifies the average squared difference between predicted and actual charges.
  - **RMSE (Root Mean Squared Error)**: Provides a more interpretable error metric by taking the square root of MSE.
  - **R² Score**: Indicates the proportion of variance in the target variable explained by the model.

## Results

- RMSE 4,454.15
- R² Score: 0.87

The model achieved a high R² Score, demonstrating its ability to predict insurance charges accurately.

## Libraries and Tools

The following libraries were used in this project:

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For visualizing the data.
- **Seaborn**: For advanced visualizations, like correlation heatmaps.
- **Scikit-learn**: For machine learning algorithms and metrics:
  - `StandardScaler`: For scaling the features.
  - `train_test_split`: To split the dataset into training and testing sets.
  - `GradientBoostingRegressor`: For building the regression model.
  - `mean_squared_error`: To calculate MSE.
  - `r2_score`: To calculate the R² Score.

