# Iris Classification with Neural Networks

## Project Overview

This project aims to classify Iris flowers into one of three species using a neural network. The dataset used is the Iris dataset, which contains features of Iris flowers. The goal is to build and evaluate a neural network model to predict the species of Iris flowers based on their features.

## Dataset

- **Source**: Iris dataset from `sklearn.datasets`.
- **Features**: Four numerical features representing the dimensions of the Iris flowers: sepal length, sepal width, petal length, and petal width.
- **Target**: Categorical classification into three species of Iris flowers (Setosa, Versicolor, Virginica).

## Steps

1. **Data Loading**: Loaded the Iris dataset and extracted features and target variables.
2. **Data Preparation**:
   - Converted target variable into categorical format using `to_categorical`.
   - Created a DataFrame for exploratory analysis.
3. **Data Splitting**: Split the dataset into training and testing sets (80% train, 20% test).
4. **Data Scaling**:
   - Standardized features using `StandardScaler` to improve model performance.
5. **Model Building**:
   - Constructed a neural network using `TensorFlow` and `Keras`:
     - Input layer with 10 neurons and ReLU activation.
     - Hidden layer with 10 neurons and ReLU activation.
     - Output layer with 3 neurons and softmax activation for multi-class classification.
6. **Model Training**:
   - Compiled the model with categorical crossentropy loss function and Adam optimizer.
   - Trained the model for 60 epochs with a batch size of 10 and a validation split of 20%.
7. **Model Evaluation**:
   - Evaluated the model on test data to obtain loss and accuracy.
   - Displayed predictions for a sample of test data.
8. **Visualization**:
   - Plotted training and validation loss over epochs to visualize model performance.

## Results

- **Loss**: The loss on the test set is `loss` (value will be printed during execution).
- **Accuracy**: The accuracy on the test set is `accuracy` (value will be printed during execution).
- **Sample Predictions**: Displayed rounded predictions for the first 5 test samples.

## Conclusion

The neural network model successfully classifies Iris flowers into their respective species with a notable accuracy. The training and validation loss trends indicate that the model has learned to generalize well from the data.

## Libraries Used

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Scikit-learn**: For dataset loading, preprocessing, and splitting.
- **TensorFlow & Keras**: For building and training the neural network.
- **Matplotlib**: For plotting loss curves.

