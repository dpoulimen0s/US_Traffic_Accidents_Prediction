# US Road Traffic Accidents Severity Prediction

## Overview

This project presents a comprehensive analysis of road traffic accidents in the United States using the Fatality Analysis Reporting System (FARS) dataset. The primary objective is to apply preprocessing techniques to enhance data quality and subsequently build and refine machine learning models to accurately predict the severity of road traffic accidents.

## Dataset

The FARS dataset consists of over 100,000 records and includes 30 distinct features related to traffic accidents. The analysis focuses on predicting injury severity using relevant features from the dataset.

## Key Steps

1. **Data Loading and Inspection**:
   - Loaded the FARS dataset and performed preliminary data inspections to understand its structure and contents.

2. **Exploratory Data Analysis (EDA)**:
   - Analyzed the distribution of injury severity and visualized the data using Seaborn and Matplotlib. 

3. **Data Preprocessing**:
   - Removed duplicated values and irrelevant categories in the target variable.
   - Applied label encoding to categorical variables and standardized feature scaling.
   - Selected important features using techniques like Chi-Squared tests and Recursive Feature Elimination (RFE).

4. **Data Splitting**:
   - Split the dataset into training, validation, and test sets to ensure robust model evaluation.

5. **Class Imbalance Handling**:
   - Resampled the training data to address any class imbalance present in the target variable.

## Model Development

- **Classifiers Implemented**:
   - Logistic Regression
   - XGBoost
   - Random Forest

Each classifier was trained and evaluated both in its untuned state and after hyperparameter tuning using grid search and randomized search techniques.

## Performance Evaluation

Model performance was evaluated using metrics such as accuracy, precision, recall, F1 score, and ROC AUC score. The final results were visualized using confusion matrices and ROC curves for a comprehensive performance comparison of the different models.

## Repository Structure

- `notebook/`: Contains Jupyter notebooks with detailed analysis and code.
- `data/`: Directory to store the FARS dataset and other relevant files.
- `README.md`: This file, providing an overview of the project.

## Prerequisites

To run this project, you will need:
- Python 3.x
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `seaborn`, `matplotlib`, `xgboost`, etc.

## Getting Started

Clone this repository and navigate to the project directory. Import the required libraries and load the dataset to start your analysis. Step through the notebooks to replicate the analysis or further your own insights into traffic accident severity prediction.
