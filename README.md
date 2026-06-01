# MNIST Handwritten Digit Classification

This project compares three neural network models for handwritten digit classification using the MNIST dataset:

1. Single-Layer Perceptron  
2. Multilayer Perceptron  
3. Convolutional Neural Network based on LeNet  

The goal of this project is to understand how model architecture affects classification performance on image data.

## Project Overview

MNIST is a handwritten digit dataset containing grayscale images of digits from 0 to 9. Each image is 28 × 28 pixels. The task is to classify each image into the correct digit class.

This project was implemented using Kaggle notebooks. Each model was trained separately, evaluated using validation metrics, and submitted to the Kaggle Digit Recognizer competition.

## Models Used

### 1. Perceptron

The perceptron is a simple single-layer linear classifier. It uses flattened pixel values as input and directly predicts one of the 10 digit classes.

### 2. Multilayer Perceptron

The MLP uses hidden layers and nonlinear activation functions. This allows the model to learn more complex patterns than a simple perceptron.

### 3. Convolutional Neural Network

The CNN uses convolution and pooling layers to learn local image patterns such as edges, curves, and strokes. This makes it more suitable for image classification tasks.

## Results

| Model | Validation Accuracy | F1-Score | Kaggle Score | Parameters |
|---|---:|---:|---:|---:|
| Perceptron | 91.76% | 0.9167 | 0.91800 | 7,850 |
| MLP | 97.12% | 0.9710 | 0.97503 | 235,146 |
| CNN / LeNet | 98.05% | 0.9803 | 0.98539 | 44,426 |

## Main Finding

The CNN achieved the best overall performance. Although the MLP had more parameters, the CNN performed better because convolutional layers are more suitable for image data.

## Repository Structure

```text
notebooks/      Kaggle notebooks for each model
submissions/    Kaggle submission CSV files
images/         Training curves, confusion matrices, and result screenshots
report.pdf      Full project report
README.md       Project explanation
