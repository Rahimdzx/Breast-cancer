# Breast Cancer Detection Using Neural Networks

This project implements a neural network model to predict breast cancer based on input data. The model is built using TensorFlow and Keras, with `Dense` layers for classification, and it uses a binary classification approach (malignant vs benign).

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Model](#model)
- [Technologies Used](#technologies-used)


## Overview
This project is aimed at detecting breast cancer by building a neural network that classifies whether a tumor is malignant or benign. The model is trained using a dataset containing various features of cell nuclei from breast cancer patients.

The neural network consists of multiple `Dense` layers with `ReLU` activations and uses `sigmoid` activation in the output layer for binary classification.

## Dataset
The dataset contains features about breast cancer such as:
- **mean radius**
- **mean texture**
- **mean perimeter**
- **mean area**
- **mean smoothness**

The target is a binary classification:
- **1**: Malignant (cancerous)
- **0**: Benign (non-cancerous)

The dataset is split into training and testing sets using an 80-20 split.

## Model
The model architecture is a feedforward neural network built using **TensorFlow**'s `Sequential` API. The model uses the following architecture:
- **Dense(128, activation='relu')**
- **Dense(64, activation='relu')**
- **Dense(16, activation='relu')**
- **Dense(1, activation='sigmoid')**

The model is compiled with:
- **Optimizer**: Adam
- **Loss Function**: Binary Cross-Entropy
- **Metrics**: Accuracy

The model is trained on the training set and evaluated on the test set.

## Technologies Used
- **Python**: Programming language
- **NumPy**: For numerical operations
- **Pandas**: For data manipulation and analysis
- **Matplotlib & Seaborn**: For data visualization
- **TensorFlow/Keras**: For building and training the neural network
- **scikit-learn**: For data preprocessing and model evaluation

