# MNIST-Digit-Classification
This repository contains a Python project demonstrating the creation, training, evaluation, and prediction using a neural network model for classifying handwritten digits from the MNIST dataset.

## Overview
The project covers the following steps:

1. Loading and Preparing Data:

   - The MNIST dataset is loaded using Keras.
   - Images are reshaped into a format suitable for neural network input.
   - Pixel values are normalized to the range [0, 1].

2. Building the Neural Network Model:
   - A simple neural network architecture is constructed using Keras Sequential API.
   - The model consists of a dense hidden layer with ReLU activation and an output layer with softmax activation.

3. Compiling the Model:
   - The model is compiled with the rmsprop optimizer, categorical_crossentropy loss function, and accuracy metric.

4. Training the Model:
   - The model is trained on the training data (train_images and train_labels) for 5 epochs with a batch size of 128.

5. Evaluating the Model:
   - The trained model is evaluated on the test data (test_images and test_labels) to compute test loss and accuracy.

6. Making Predictions:
   - Predictions are made on new data (test_images) using the trained model to classify digits.
   - Probability distributions are generated for each input image, and the class with the highest probability is chosen as the predicted digit.
