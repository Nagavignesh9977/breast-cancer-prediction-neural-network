
# Breast Cancer Prediction using Neural Networks

## Overview
Breast cancer is one of the most common cancers affecting women worldwide. 
Early detection can significantly improve survival rates. 

This project implements a **Neural Network model using TensorFlow and Keras** to predict whether a tumor is **malignant or benign** based on medical features.

The model learns patterns from historical diagnostic data and provides predictions that can support medical analysis.

---

## Problem Statement
Breast cancer diagnosis requires analyzing several medical parameters. 
Manual analysis can be time-consuming and error-prone.

The goal of this project is to build a **machine learning model that predicts breast cancer using neural networks**, improving diagnostic assistance.

---

## Objective
- Build a neural network for cancer prediction
- Train the model using medical dataset features
- Classify tumors into **Benign (1) or Malignant (0)**
- Evaluate the model using accuracy metrics

---

## Dataset
The dataset used is the **Breast Cancer Wisconsin Dataset**.

Features include:

- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Symmetry
- Fractal Dimension

Target variable:
- **Malignant → 0**
- **Benign → 1**

Dataset size:
- 569 samples
- 30 features

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Scikit-learn
- Matplotlib

---

## Model Architecture

The Neural Network consists of:

Input Layer  
↓  
Flatten Layer  
↓  
Dense Layer (20 neurons, ReLU activation)  
↓  
Dense Layer (10 neurons, ReLU activation)  
↓  
Output Layer (1 neuron, Sigmoid activation)

---

## Model Parameters

Optimizer: Adam  
Loss Function: Binary Crossentropy  
Metric: Accuracy  
Epochs: 50  
Batch Size: 32  

Model compilation:

```python
model.compile(
    optimizer='adam',
    loss='binary_crossentropy',
    metrics=['accuracy']
)
## flow chart of the project
Import Libraries
        ↓
Load Dataset
        ↓
Data Preprocessing
        ↓
Train Test Split
        ↓
Build Neural Network
        ↓
Compile Model
        ↓
Train Model
        ↓
Evaluate Model
        ↓
Prediction
