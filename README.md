
# Credit Card Fraud Detection

This project aims to develop a machine learning model to detect fraudulent credit card transactions. The model is trained using a publicly available dataset and includes various techniques for preprocessing, feature selection, and model evaluation.

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Modeling](#modeling)
- [Results](#results)
- [Usage](#usage)
- [Contributions](#contributions)

## Introduction

Credit card fraud is a significant problem that leads to billions of dollars in losses every year. This project focuses on building a classification model that can predict whether a given transaction is fraudulent based on historical data.

## Dataset

The dataset used in this project is the [Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud) available on Kaggle. It contains transactions made by European cardholders in September 2013. The dataset consists of 284,807 transactions, where 492 are labeled as fraudulent.

Key characteristics of the dataset:
- Highly imbalanced, with only 0.172% of transactions being fraudulent.
- All features except for time and amount are anonymized to protect sensitive information.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Arkoprovo08/Credit-Card-Fraud-Detection.git
   cd Credit-Card-Fraud-Detection
   ```

2. Install the required Python packages:

   ```bash
   pip install -r requirements.txt
   ```

## Modeling

The project includes the following steps:
1. **Data Preprocessing**: Handle missing values, normalize features, and balance the dataset using techniques like SMOTE (Synthetic Minority Over-sampling Technique).
2. **Feature Selection**: Select the most relevant features using methods such as correlation analysis.
3. **Modeling**: Several machine learning models are trained and evaluated, including:
   - Logistic Regression
   - Random Forest
4. **Evaluation**: The models are evaluated using accuracy, precision, recall and F1-score.

## Results

The performance of the best model is summarized below:

| Model               | Training Accuracy | Testing Accuracy  |
|---------------------|-------------------|-------------------|
| Logistic Regression | 94.14%            | 93.91%            |

## Usage

To use the model for predicting fraud on a new dataset, follow these steps:

1. Prepare the input data in the same format as the original dataset (including anonymized features).
2. Run the prediction script:

   ```bash
   python predict.py --input_file <path_to_input_file>
   ```

3. The script will output whether each transaction is fraudulent or not.

## Contributions

Contributions are welcome! Please open an issue or submit a pull request for any improvements.
