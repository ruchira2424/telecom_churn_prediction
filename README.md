# Telecom Customer Churn Prediction with Machine Learning

This repository contains a Jupyter notebook for predicting customer churn in a telecom company using machine learning. The analysis is based on the BigML Telecom Churn dataset, which includes customer usage patterns, plans, and demographic data. The goal is to identify factors leading to churn and build a predictive model to help reduce customer attrition.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Overview
Customer churn is a critical issue for telecom companies, leading to revenue loss. This project performs:
- Data preprocessing (e.g., label encoding, dropping irrelevant columns like State and Area Code).
- Model training (using a tree-based classifier to predict churn).
- Feature importance analysis to identify key predictors (e.g., total day minutes, customer service calls).
- Model evaluation with a confusion matrix.

The notebook demonstrates end-to-end workflow from data loading to visualization.

## Dataset
The dataset is sourced from [BigML Telecom Churn](https://bigml.com/shared/dataset/7f9cbba4ab266e120c2f2b4092b83220) and split into:
- **Training Set**: `churn-bigml-80.csv` (80% of data, ~2666 rows).
- **Testing Set**: `churn-bigml-20.csv` (20% of data, ~667 rows).

Key columns include:
- Account length, International plan, Voice mail plan, Total day/eve/night/intl minutes/calls/charges, Customer service calls, Churn (target: True/False).

**Note**: If the CSV files are not in this repo, download them from the BigML link or Kaggle equivalent and place them in the root directory.

## Features
- **Preprocessing**: Dropping unnecessary columns, label encoding for categorical features (e.g., International plan, Voice mail plan), and converting the target (Churn) to numeric.
- **Modeling**: A tree-based model (e.g., Random Forest or Gradient Boosting) is trained on the preprocessed dta.
- **Visualization**:
  - Bar plot for feature importances in predicting churn.
  - Heatmap for the confusion matrix to evaluate model performance.
- **Libraries Used**:
  - Data Manipulation: Pandas, NumPy
  - Modeling: Scikit-learn (LabelEncoder, model training, confusion_matrix)
  - Visualization: Matplotlib, Seaborn

## Installation
1. Clone the repository: git clone https://github.com/ruchira2424/telecom-churn-prediction.git
cd telecom-churn-prediction

   
