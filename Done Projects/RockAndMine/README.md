# Sonar Data Classification with Random Forest

## Project Overview

This project involves classifying sonar data to detect rocks and mines using a Random Forest classifier. The dataset used contains sonar readings, and the goal is to build and evaluate a model to predict whether a sonar reading corresponds to a rock or a mine.

## Dataset

- **Source**: `sonardata.csv`
- **Features**: Various numerical features representing sonar readings.
- **Target**: Categorical classification into two classes: Rock (`R`) or Mine (`M`).

## Steps

1. **Data Import**:
   - Loaded the sonar dataset from a CSV file.

2. **Data Splitting**:
   - Split the dataset into features (`X`) and target (`Y`).
   - Further split the data into training and testing sets (80% train, 20% test).

3. **Model Training**:
   - Trained a Random Forest classifier with 150 estimators on the training data.

4. **Model Evaluation**:
   - Made predictions on the test set and calculated the accuracy score.

5. **Testing with New Data**:
   - Created a sample input data point and predicted its class using the trained model.
   - Displayed the prediction and interpreted the result.

## Results

- **Accuracy**: The accuracy on the test set is `0.86`.
- **Prediction**: For the sample input data, the model predicted `Rock` or `Mine`
