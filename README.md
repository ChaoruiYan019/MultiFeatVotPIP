# Proinflammatory Peptide Classification using Machine Learning

This repository contains code for classifying proinflammatory peptides (PIPs) using machine learning models. The dataset consists of peptide sequences labeled as **proinflammatory (1)** and **non-proinflammatory (0)**. We used **Random Forest** and **Graph Neural Networks (GNN)** for classification.

## Project Overview

Peptides that induce proinflammatory cytokines (PIPs) play a significant role in the inflammatory response and are crucial for understanding various diseases. This project aims to predict whether a given peptide is proinflammatory or not based on its sequence.

## Datasets

The dataset consists of peptide sequences and their corresponding labels. The sequences are analyzed using two models:
1. **Random Forest (RF) Classifier**: A traditional machine learning model that performs well with structured feature sets.
2. **Graph Neural Networks (GNN)**: A more advanced method leveraging the relationships between amino acids within peptide sequences.

- **Train Dataset**: 2872 samples
- **Test Dataset**: 342 samples

## Models Used

### 1. **Random Forest Classifier**
Random Forest is an ensemble learning method that constructs multiple decision trees to improve the accuracy and robustness of predictions.

### 2. **Graph Neural Networks (GNN)**
GNN models leverage the structure of the peptide sequences, considering the relationships between amino acids and their spatial configurations.

## Results

### Random Forest Model
- **Confusion Matrix**:  
  ```plaintext
  [[135  36]  
   [108  63]]
## Results

### Random Forest Model
- **Test Accuracy**: 57.89%
- **Test MCC**: 0.17

### Graph Neural Network Model
- **Test Accuracy**: 58.77%
- **Test MCC**: 0.18
