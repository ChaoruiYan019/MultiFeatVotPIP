# Peptide Classification Model

This project focuses on classifying peptide sequences as proinflammatory or non-proinflammatory using various machine learning models. The models are trained on a dataset containing peptide sequences labeled as either 0 (non-proinflammatory) or 1 (proinflammatory). The goal is to evaluate and compare the performance of several classification algorithms, including SVM, Naive Bayes, Random Forest, and Gradient Boosting.

## Project Structure

- `data/`: Directory containing the preprocessed data.
- `models/`: Directory containing the trained models.
- `scripts/`: Python scripts for model training, evaluation, and preprocessing.
- `notebooks/`: Jupyter notebooks for exploratory analysis, data visualization, and model experimentation.
- `requirements.txt`: Python dependencies for the project.
- `README.md`: Documentation for the project.

## Models Used

1. **Support Vector Machine (SVM)**: A classifier for handling binary classification tasks.
2. **Naive Bayes**: A simple probabilistic classifier based on Bayes' theorem.
3. **Random Forest**: A robust ensemble method for classification using multiple decision trees.
4. **Gradient Boosting**: An ensemble technique that builds models sequentially, focusing on mistakes made by previous models.

## Results Summary

### SVM Model
- **Validation Accuracy**: 57.39%
- **Test Accuracy**: 50%
- **Validation MCC**: 0.0
- **Test MCC**: 0.0
- **Precision/Recall Issue**: Model performs well for class 0 (non-proinflammatory) but fails to predict class 1 (proinflammatory), leading to poor performance.

### Naive Bayes Model
- **Validation Accuracy**: 57.39%
- **Test Accuracy**: 50%
- **Validation MCC**: 0.0
- **Test MCC**: 0.0
- **Precision/Recall Issue**: Similar to the SVM model, it shows poor recall for class 1 and performs well only for class 0.

### Random Forest Model
- **Validation Accuracy**: 57.39%
- **Test Accuracy**: 50%
- **Validation MCC**: 0.0
- **Test MCC**: 0.0
- **Precision/Recall Issue**: The model is overfitting, showing high accuracy for class 0 and completely failing for class 1.

### Gradient Boosting Model
- **Validation Accuracy**: 57.39%
- **Test Accuracy**: 50%
- **Validation MCC**: 0.0
- **Test MCC**: 0.0
- **Precision/Recall Issue**: Similar performance to the Random Forest, with high accuracy for class 0 but no predictive ability for class 1.

## Known Issues

- **Overfitting**: All models have demonstrated overfitting, where they perform well on the training data but fail to generalize to the test data. This is particularly evident in the case of class 1 (proinflammatory), where models fail to predict this class.
  
- **Class Imbalance**: The models face challenges in predicting the minority class (proinflammatory), leading to precision and recall issues.

## Potential Solutions

- **Resampling Techniques**: Consider using oversampling (e.g., SMOTE) for the minority class or undersampling for the majority class.
- **Class Weights Adjustment**: Update model parameters to account for class imbalance, such as adjusting class weights in SVM and Random Forest models.
- **Alternative Metrics**: Use metrics such as F1-score or MCC (Matthews Correlation Coefficient) instead of accuracy for more balanced evaluation.
- **Hyperparameter Tuning**: Perform grid search or random search for hyperparameter optimization to improve model performance.


## Get Involved

If you have suggestions or solutions to improve this model's performance or any other ideas, feel free to open an issue or submit a pull request. We are looking for ways to address the overfitting issue and improve the model's ability to predict class 1 (proinflammatory) correctly.


