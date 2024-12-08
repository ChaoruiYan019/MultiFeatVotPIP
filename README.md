# Peptide Sequence Classification with GNN and Traditional Models

This project aims to classify peptide sequences as proinflammatory or non-proinflammatory using various machine learning models, including traditional models like SVM, Naive Bayes, and Random Forest, as well as a Graph Neural Network (GNN). The dataset contains peptide sequences labeled as either proinflammatory (`1`) or non-proinflammatory (`0`).

## Models Evaluated:

1. **Support Vector Machine (SVM)**:
   - Accuracy on test data: 50%
   - MCC score: 0.00
   - The SVM model performs well on one class (non-proinflammatory) but fails to predict the other class (proinflammatory).

2. **Naive Bayes**:
   - Accuracy on test data: 50%
   - MCC score: 0.00
   - Similar to the SVM model, Naive Bayes shows poor performance in classifying the proinflammatory class.

3. **Random Forest**:
   - Accuracy on test data: 50%
   - MCC score: 0.00
   - Random Forest also demonstrates overfitting, showing perfect performance on the training data but poor generalization on test data.

4. **Graph Neural Network (GNN)**:
   - Training Accuracy: 100%
   - Test Accuracy: 50%
   - MCC score: 0.00
   - The GNN model achieved 100% training accuracy but also overfitted. It only classifies the non-proinflammatory class correctly, resulting in 50% test accuracy.

## Observations:
- **Overfitting**: All models, including the GNN, suffer from overfitting, showing perfect performance on the training data but poor generalization to the test data.
- **Imbalanced Classes**: The dataset is imbalanced, with a larger number of non-proinflammatory peptides compared to proinflammatory peptides, which might be contributing to the bias in predictions.

## Solutions Needed:
- **Overfitting Solutions**: Help is needed to address the overfitting issue in all models. Suggestions on regularization techniques or strategies to improve generalization would be appreciated.
- **Class Imbalance**: How to handle the class imbalance to ensure that the model doesn’t bias toward the majority class (non-proinflammatory).
- **Evaluation Metrics**: We are also looking for suggestions to improve evaluation metrics for better understanding of model performance, particularly the MCC score, which is currently very low.

## Get Involved

If you have suggestions or solutions to improve this model's performance or any other ideas, feel free to open an issue or submit a pull request. We are looking for ways to address the overfitting issue and improve the model's ability to predict class 1 (proinflammatory) correctly.


