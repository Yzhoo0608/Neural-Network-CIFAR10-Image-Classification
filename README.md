# Neural Network Image Classification

## Overview

This project develops a binary image classification model to distinguish between **Coin** and **Not Coin** images. Image datasets from multiple sources are combined and preprocessed before training and evaluating two neural network architectures: a baseline Neural Network and a Convolutional Neural Network (CNN).

## Technologies

- Python
- TensorFlow / Keras
- NumPy
- Matplotlib
- Scikit-learn

## Methodology

1. **Dataset Integration:** Combine image datasets from multiple sources into a unified dataset.
2. **Image Preprocessing:** Resize images to 224 × 224 pixels and prepare labels for binary classification.
3. **Baseline Model:** Build a fully connected neural network using Flatten and Dense layers.
4. **CNN Model:** Introduce convolutional and pooling layers to learn spatial image features.
5. **Evaluation:** Compare model performance using accuracy, loss, precision, recall, F1-score, and a confusion matrix.

## Baseline Neural Network

The initial model consists of:

- Flatten layer with input shape `(224, 224, 3)`
- Dense layer with 256 neurons and sigmoid activation
- Dense layer with 50 neurons and sigmoid activation
- Output layer with 1 neuron and sigmoid activation

The baseline achieved limited performance, motivating the development of a CNN.

## Results

| Metric | Baseline NN | CNN |
|---|---:|---:|
| Training Accuracy | 56.01% | 100% |
| Validation Accuracy | 52.25% | 100% |
| Training Loss | 0.6876 | 0.0000205 |
| Validation Loss | 0.6923 | 0.0000379 |

The CNN achieved **100% accuracy on the reported test set of 445 images**, with precision, recall, and F1-score of 1.00 for both classes.




