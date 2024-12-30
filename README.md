# Peptide Sequence Analysis Using Machine Learning Models

This project focuses on classifying peptide sequences into proinflammatory (label: 1) and non-proinflammatory (label: 0) categories using various machine learning models and feature extraction techniques. The models are evaluated using performance metrics including **accuracy**, **confusion matrix**, and **Matthew's Correlation Coefficient (MCC)** to ensure robust performance evaluation.

## Project Highlights
- Implemented **TF-IDF** feature extraction with mono-, bi-, and tri-grams as well as gapped bigrams and trigrams.
- Explored multiple machine learning models:
  -  RandomForestClassifier

## Dataset Description
The dataset includes peptide sequences labeled as:
- `1`: Proinflammatory
- `0`: Non-proinflammatory

Columns:
- **peptide_sequence**: The peptide sequence to classify.
- **label**: Binary classification label.

## Feature Extraction
### TF-IDF
- Features are generated using:
  - **Monograms**
  - **Bigrams**
  - **Trigrams**
  - **Gapped bigrams** (e.g., `AB_X_CD`)
  - **Gapped trigrams** (e.g., `AB_X_Y_CD`)
- TF-IDF scores reflect the importance of sequence patterns in the corpus, aiding in distinguishing proinflammatory from non-proinflammatory sequences.

## Model Results
###  RandomForestClassifier
- **Validation Accuracy**: 65.73%
- **Test Accuracy**: 59.06%
- **Validation MCC**: 0.28
- **Test MCC**: 0.19


