# Kaggle Digit Recognizer — Handwritten Digit Classification

## Overview

This project focuses on handwritten digit classification using machine learning and deep learning.

I participated in the [Kaggle Digit Recognizer competition](https://www.kaggle.com/competitions/digit-recognizer) and compared multiple classification models to improve prediction accuracy.

**Final Kaggle Public Leaderboard Accuracy: 99.285%**

**Leaderboard Rank: 255 (October 2026)**

## Dataset

- Dataset: MNIST-based handwritten digit images
- Training samples: 42,000
- Test samples: 28,000
- Image size: 28 × 28 pixels
- Classes: Digits 0–9

The pixel values were normalized from 0–255 to 0–1.

The training data was split into 80% training and 20% validation sets using stratified sampling.

## Models and Results

| Model | Validation Accuracy |
|---|---:|
| Logistic Regression | 91.30% |
| Multi-Layer Perceptron (MLP) | 97.35% |
| Convolutional Neural Network (CNN) | 98.92% |
| CNN with Data Augmentation | **99.23%** |

The final model achieved **99.285% accuracy on the Kaggle Public Leaderboard**.

## Methodology

### 1. Logistic Regression

Implemented logistic regression as a baseline classification model.

Evaluated performance using accuracy and a confusion matrix to identify frequently misclassified digits.

### 2. Multi-Layer Perceptron (MLP)

Implemented an MLP with two hidden layers (128 and 64 neurons).

Improved validation accuracy from 91.30% to 97.35%.

### 3. Convolutional Neural Network (CNN)

Implemented a CNN using TensorFlow/Keras with convolutional layers, max pooling, dropout, and a fully connected classification layer.

Achieved 98.92% validation accuracy.

### 4. Data Augmentation

Applied random rotation, translation, and zoom transformations to training images.

This improved the final validation accuracy to 99.23%.

Early stopping was used to reduce overfitting.

## Key Learnings

- Compared traditional machine learning and deep learning approaches.
- Analyzed classification errors using confusion matrices.
- Improved generalization performance through data augmentation.
- Evaluated overfitting by comparing training and validation accuracy.
- Created a submission file containing predictions for 28,000 test images.

## Technologies

- Python
- NumPy
- pandas
- Matplotlib
- scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

## Notebook

[View the Jupyter Notebook](数字認識.ipynb)

## Future Improvements

- Analyze misclassified images from the final CNN.
- Experiment with batch normalization and learning-rate scheduling.
- Evaluate model robustness across multiple random seeds.

## Competition

[Kaggle — Digit Recognizer](https://www.kaggle.com/competitions/digit-recognizer)
