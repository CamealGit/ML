# Breast Cancer Classification with Neural Networks

## Project Overview

This project focuses on classifying breast cancer tumors using a neural network model. The dataset utilized is the Breast Cancer Wisconsin dataset, which includes various features of tumors. The aim is to build and evaluate a neural network to predict whether a tumor is malignant or benign based on these features.

## Dataset

- **Source**: Breast Cancer Wisconsin dataset from `scikit-learn`.
- **Features**: 30 numerical features related to tumor characteristics.
- **Target**: Binary classification (0 = malignant, 1 = benign).

## Steps

1. **Data Loading**: Imported the dataset and converted it into a pandas DataFrame.
2. **Data Exploration**: Analyzed and described the dataset. Calculated summary statistics and grouped data by the target variable.
3. **Data Preprocessing**:
   - Standardized numerical features using `StandardScaler`.
   - Split the data into training and testing sets.
4. **Model Building**:
   - Constructed a neural network using `TensorFlow` and `Keras`.
   - The network includes:
     - An input layer that flattens the data.
     - A hidden layer with 20 neurons and ReLU activation.
     - An output layer with 2 neurons and sigmoid activation.
5. **Model Training**:
   - Compiled the model with the Adam optimizer and sparse categorical crossentropy loss function.
   - Trained the model for 20 epochs.
6. **Evaluation**:
   - Evaluated the model on the test data to assess its accuracy.
   - Plotted accuracy trends over epochs for both training and validation data.
7. **Prediction**:
   - Made predictions on test data and new sample data.
   - Converted the predictions into binary labels (malignant or benign).

## Results

- **Model Accuracy**: Achieved 0.97 high accuracy on the test dataset.
- **Example Prediction**: Demonstrated the model’s capability to classify new tumor data correctly.

## Conclusion

The neural network model effectively classifies breast cancer tumors with high accuracy, showcasing the potential of deep learning for medical diagnostics. This project highlights the process of building, training, and evaluating a neural network for a binary classification problem.

---

Libraries Used

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations and array handling.
- **Scikit-learn**: For dataset loading, preprocessing, and splitting.
- **TensorFlow**: For building and training the neural network.
- **Keras**: For high-level neural network API within TensorFlow.
- **Matplotlib**: For plotting training and validation accuracy.


