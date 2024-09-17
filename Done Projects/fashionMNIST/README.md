# Fashion MNIST Classification with Convolutional Neural Network
This project demonstrates the use of a Convolutional Neural Network (CNN) for classifying images from the Fashion MNIST dataset. The dataset consists of grayscale images of 10 different fashion categories.

## Overview

The project uses TensorFlow and Keras to build and train a CNN model. The model is designed to classify images into one of 10 categories with high accuracy. Key components of the model include convolutional layers, max-pooling layers, and dense layers.

## Components

1. **Libraries**:
   - `tensorflow`: For building and training the neural network.
   - `numpy`: For data manipulation.
   - `matplotlib`: For plotting (if needed).
   - `pandas`: For data handling (if needed).
   - `ImageDataGenerator`: For data augmentation.
   - `EarlyStopping`: To prevent overfitting by stopping training early.

2. **Data Preparation**:
   - **Loading Data**: The Fashion MNIST dataset is loaded using `tensorflow.keras.datasets.fashion_mnist`.
   - **Normalization**: The pixel values of the images are normalized to the range [0, 1].
   - **Reshaping**: The images are reshaped to include a channel dimension, making them compatible with the CNN.

3. **Data Augmentation**:
   - **ImageDataGenerator**: Applied transformations include rotation, width and height shifts, shearing, zooming, and horizontal flipping to improve model generalization.

4. **Model Architecture**:
   - **Convolutional Layers**: 
     - 32 filters with a kernel size of (3, 3) followed by max pooling.
     - 64 filters with a kernel size of (3, 3) followed by max pooling.
   - **Flatten Layer**: Flattens the 3D output of the convolutional layers to 1D.
   - **Dense Layers**:
     - 64 units with ReLU activation.
     - 10 units with softmax activation for classification.

5. **Model Training**:
   - **Optimizer**: Adam optimizer.
   - **Loss Function**: Sparse categorical crossentropy.
   - **Early Stopping**: Monitors validation loss to stop training if no improvement is observed for 3 consecutive epochs.

6. **Evaluation**:
   - The model is evaluated on the test set to determine its accuracy and loss.
## Results
- **Test Accuracy:** 0.86
- **Test Loss:** 0.40
