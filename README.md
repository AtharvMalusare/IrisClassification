# Iris Flower Classification

This project classifies the famous **Iris flower dataset** using two models:
1. **Support Vector Machine (SVM)** with Radial Basis Function (RBF) kernel and GridSearchCV for hyperparameter tuning.
2. **Neural Network** implemented with TensorFlow/Keras.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Models Used](#models-used)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

The Iris dataset contains 150 samples of Iris flowers with 4 features:
- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

The goal of this project is to classify these flowers into three species:
- Iris Setosa
- Iris Versicolor
- Iris Virginica

## Dataset

The dataset consists of 150 samples and 5 columns:
- `SepalLengthCm`, `SepalWidthCm`, `PetalLengthCm`, `PetalWidthCm`: Features of the flowers.
- `Species`: The target label (Iris-setosa, Iris-versicolor, Iris-virginica).

## Models Used

### 1. Support Vector Machine (SVM)
- **Kernel**: Radial Basis Function (RBF)
- **Hyperparameter Tuning**: Grid Search with cross-validation using `C` and `gamma` values.
- Achieved an accuracy of **100%** on the test data.

### 2. Neural Network
- A simple **Sequential** model built with TensorFlow/Keras.
- **Architecture**:
  - Input Layer: 64 neurons, ReLU activation
  - Hidden Layer: 32 neurons, ReLU activation
  - Output Layer: 3 neurons (one for each class), softmax activation.
- Achieved high accuracy after training with **60 epochs**.

## Installation

To run this project locally, clone the repository and install the dependencies:

```bash
git clone https://github.com/Sudo_User/iris-flower-classification.git
cd iris-flower-classification
pip install -r requirements.txt
