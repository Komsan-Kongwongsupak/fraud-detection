# Credit Card Fraud Detection Dataset

## Overview

This dataset contains anonymized credit card transactions labeled as fraudulent or genuine. It is commonly used for machine learning and data analysis tasks related to fraud detection.

## Data Source

- **Original Source**: [Credit Card Fraud Detection Dataset on Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## Dataset Details

- **Number of Instances**: 284,807 transactions
- **Number of Features**: 31
- **Class Distribution**:
  - **Non-Fraudulent Transactions (Class 0)**: 284,315
  - **Fraudulent Transactions (Class 1)**: 492

## Feature Information

The dataset consists of numerical features resulting from a PCA transformation to protect confidentiality. The features are:

- **V1, V2, ..., V28**: Principal components obtained from PCA.
- **Time**: The elapsed time in seconds between this transaction and the first transaction in the dataset.
- **Amount**: The transaction amount.
- **Class**: The target variable (0 for non-fraudulent, 1 for fraudulent).

## Data Characteristics

- **Imbalance**: The dataset is highly imbalanced, with fraudulent transactions accounting for only about 0.172% of all transactions.
- **Anonymization**: Due to confidentiality, original feature names and detailed information are not provided.

## Usage

This dataset is suitable for:

- **Anomaly Detection**: Identifying rare fraudulent transactions.
- **Classification**: Building models to classify transactions as fraudulent or genuine.
- **Imbalanced Learning**: Experimenting with techniques to handle imbalanced datasets.

## Acknowledgements

The dataset is provided by [Machine Learning Group - ULB](https://www.ulb.ac.be/di/map/adalpozz/data/creditcardfraud/). 