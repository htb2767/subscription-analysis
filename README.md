# Subscription Prediction Project

## Overview

This project focuses on predicting customer subscriptions based on app behavior analysis. The goal is to understand user interactions within the mobile app and leverage machine learning to predict whether a user will subscribe to the premium service or not. The analysis includes exploratory data analysis (EDA), feature engineering, model building, and hyperparameter tuning.

## Table of Contents

- [Dataset](#dataset)
- [Data Pre-Processing](#data-pre-processing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Building](#model-building)
- [Model Tuning](#model-tuning)
- [Results and Insights](#results-and-insights)
- [Usage](#usage)

## Dataset

The dataset (`new_appdata10.csv`) is used for training and testing the machine learning model. It includes various features related to user behavior within the mobile app, such as time spent on screens, interactions with specific features, and timestamps of app usage.

## Data Pre-Processing

- The dataset is loaded and pre-processed to handle missing values, format date columns, and engineer relevant features.
- The training set is split into independent variables (X) and the response variable (y).
- Optional: The training set is balanced to handle class imbalance (code is commented out).

## Exploratory Data Analysis (EDA)

- Initial data exploration is performed, including displaying the first few rows, summary statistics, and visualizing numerical features.
- Histograms and correlation matrices are created to understand the distribution of features and their relationships with the response variable.

## Model Building

- Logistic Regression with L1 penalty is chosen as the initial model for predicting subscriptions.
- The model is trained on the training set and evaluated on the test set using various metrics, including accuracy, precision, recall, and F1 score.

## Model Tuning

- Grid search is conducted to tune hyperparameters, including regularization strength (C) and penalty type (L1 or L2).
- Two rounds of grid search are performed with different hyperparameter ranges.

## Results and Insights

- The final results include the confusion matrix, accuracy, and other evaluation metrics.
- Coefficients of the logistic regression model are analyzed to gain insights into feature importance.

## Usage

To reproduce or extend the analysis, follow these steps:

1. Clone the repository: `git clone https://github.com/htb2767/subscription-analysis`
2. Install required dependencies: `pip install -r requirements.txt`
3. Run the Jupyter Notebook or Python scripts for data preprocessing, EDA, model building, and tuning.

