# Handwritten Digits Classification

## Introduction
builded a machine learning model to classify handwritten digits into the correct digit class they belong to. MNIST is a dataset consisting of a collection of 28x28 grayscale images of handwritten digits (0 through 9) along with their corresponding labels.

## Dataset
The MNIST dataset is loaded using TensorFlow's Keras API. It contains 60,000 training images and 10,000 test images. Each image is a single-channel (grayscale) image with pixel values representing the intensity of the pixels.

## Preprocessing
The pixel values of the images are scaled between 0 and 1 to improve accuracy. The 2D image arrays are flattened into 1D arrays to feed into the neural network model.

## Model Architecture
A neural network model is created using Keras Sequential API. The initial model consists of a single dense layer with 10 neurons, representing the digits from 0 to 9, using sigmoid activation. The model is compiled with the Adam optimizer and sparse categorical crossentropy loss function.

## Training and Evaluation
The model is trained on the training data for 5 epochs. Evaluation is performed on the test data to measure accuracy. Confusion matrix visualization is used to analyze the model's performance.

## Model Improvement
To improve performance, a hidden layer with 100 neurons and ReLU activation is added. The model is trained for an additional 5 epochs. Evaluation shows an accuracy improvement from 0.9252 to 0.9770.
