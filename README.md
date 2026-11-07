# Smoking Status Prediction Using Machine Learning

## Project Overview

This project aims to predict smoking status using machine learning classification algorithms. The study uses the **Smokers Health Data** dataset obtained from Kaggle.

Two classification models, Logistic Regression and Random Forest, are implemented and compared to evaluate their performance in predicting smoking status.

The main objective is to investigate how effectively these algorithms classify individuals based on the available dataset features and to determine which model provides better predictive performance.

## Dataset

- **Dataset Name:** Smokers Health Data
- **Source:** [Kaggle – Smokers Health Data](https://www.kaggle.com/datasets/jaceprater/smokers-health-data)
- **Data Format:** CSV
- **Task:** Binary classification (depending on the target variable encoding)
- **Target Variable:** Smoking status column

The dataset contains individual records and features used to predict smoking status. The dataset structure, feature names, number of observations, and class distribution are examined during the data analysis stage.

## Machine Learning Models

Two classification algorithms are used in this project:

### 1. Logistic Regression

Logistic Regression is used as a baseline classification model. It estimates the probability of an observation belonging to a particular class using a logistic function.

### 2. Random Forest Classifier

Random Forest is an ensemble learning algorithm that combines multiple decision trees to make predictions. It can capture more complex relationships between input features.

Both models are trained and evaluated using the same data split to ensure a fair comparison.

## Data Preprocessing

The preprocessing stage includes:

- Checking missing values.
- Separating numerical and categorical features.
- Handling missing numerical and categorical values.
- Applying feature scaling to numerical variables where appropriate.
- Encoding categorical variables into numerical representations.
- Splitting the dataset into training and testing sets.

A preprocessing pipeline is used to ensure consistent transformations.

## Model Evaluation

The models are evaluated using the following classification metrics:

| Metric | Description |
|---|---|
| Accuracy | Measures the overall proportion of correct predictions. |
| Precision | Measures how many positive predictions are correct. |
| Recall | Measures how many actual positive cases are identified. |
| F1 Score | Represents the harmonic mean of precision and recall. |
| Confusion Matrix | Shows correct and incorrect predictions for each class. |

Training and validation performance are also compared to investigate potential overfitting.

## Overfitting Analysis

The Random Forest model is further examined by comparing training and validation accuracy across different numbers of decision trees.

This analysis helps determine whether the model performs significantly better on training data than on unseen data.

## Project Structure

```text
Smoking-Status-Prediction/
│
├── dataset/
│   └── smokers_health_data.csv
│
├── notebooks/
│   └── smoking_prediction.ipynb
│
├── README.md
└── requirements.txt
```

*The folder structure can be adjusted according to the actual project files.*

## Technologies and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- KaggleHub

## Installation

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn kagglehub
```

Download the dataset through KaggleHub or provide the CSV file locally, then run the project notebook or Python script.

## Conclusion

This project provides a comparative study of Logistic Regression and Random Forest for smoking status classification.

By evaluating both models with multiple classification metrics and examining potential overfitting, the project aims to identify a model that achieves reliable performance on unseen data.

## Future Improvements

- Hyperparameter optimization.
- Cross-validation.
- Testing additional classification algorithms.
- Feature importance analysis.
- Further investigation of class imbalance.
- Improving model generalization.

## Author

Machine Learning Classification Project
