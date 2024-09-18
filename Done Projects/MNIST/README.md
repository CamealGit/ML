# Handwritten Digit Classification with Convolutional Neural Networks

## Project Overview

This project aims to classify handwritten digits using Convolutional Neural Networks (CNNs). The dataset used is the MNIST dataset, which contains images of handwritten digits. The goal is to build and evaluate a CNN model to predict the digit in each image based on its features.

## Dataset

- **Source**: MNIST dataset.
- **Features**: 28x28 pixel grayscale images of handwritten digits (0-9).
- **Target**: Categorical classification into 10 digit classes (0-9).

## Steps

1. **Data Loading**: Loaded the training and test datasets from CSV files.
2. **Data Preparation**:
   - Separated features and labels from the training data.
   - Normalized pixel values of images to be between 0 and 1.
3. **Data Splitting**: Split the training data into training and validation sets (80% train, 20% validation).
4. **Data Reshaping**:
   - Reshaped images into 4D format suitable for CNN input (28x28 pixels with 1 color channel).
5. **Data Visualization**:
   - Visualized sample images from the training data to understand the dataset.
6. **Model Building**:
   - Constructed a CNN using `TensorFlow` and `Keras`:
     - Convolutional layers with ReLU activation.
     - MaxPooling layers for downsampling.
     - BatchNormalization layers to stabilize learning.
     - Dense layers for classification.
7. **Model Training**:
   - Compiled the model with categorical crossentropy loss function and Adam optimizer.
   - Trained the model for 10 epochs with a batch size of 32 and a validation split of 20%.
8. **Model Evaluation**:
   - Evaluated the model on the test set to obtain accuracy.
   - Displayed sample predictions and their corresponding images.
9. **Visualization**:
   - Plotted training and validation accuracy over epochs to visualize model performance.

## Results

- **Test Accuracy**: 0.99
- **Training Details**: 
  - Loss: 0.0558
  - Accuracy: 0.9867

## Conclusion

The Convolutional Neural Network model successfully classifies handwritten digits with a high accuracy of 0.99. The training and validation accuracy trends indicate that the model has effectively learned to generalize from the data.

## Libraries Used

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization and plotting.
- **TensorFlow & Keras**: For building and training the CNN.
- **Scikit-learn**: For data splitting and evaluation metrics.

