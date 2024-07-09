# Predicting Vaccination Likelihood

## Overview

This repository contains the code and data used to analyze vaccination probabilities. The primary goal of this project is to extract and evaluate various features from our dataset and use them to create models to predict whether or not an individual received an H1N1 or seasonal vaccine.

## Business Problem

The project aims to predict vaccination outcomes based on extracted features from a dataset. By analyzing these features, we develop machine learning models to predict the likelihood of an individual receiving either the H1N1 or seasonal flu vaccine.

### Table of Contents

- [Overview](#overview)
- [Business Problem](#business-problem)
- [Data Sources](#data-sources)
- [Installation](#installation)
- [Analysis and Results](#analysis-and-results)
  - [Feature Extraction](#feature-extraction)
  - [Model Creation](#model-creation)
  - [Evaluation](#evaluation)
- [Conclusion](#conclusion)

## Data Sources

We used data from the National 2009 H1N1 Flu Survey dataset, which includes anonymized features related to individuals' demographics, health-related variables, and past behaviors regarding vaccination. https://www.cdc.gov/nchs/index.htm

## Installation

To run the project, follow these steps:

1. Clone the repository: git clone https://github.com/Gfatouras/Phase3.git
2. Install dependencies: pip install -r requirements.txt
   
## Analysis and Results

### Feature Extraction

Initial steps involved extracting 35 relevant features from the dataset, including demographic information, health-related variables, and opinions related to vaccines. Feature selection techniques were applied to identify the most predictive variables.

### Model Creation

Multiple machine learning models were developed using the extracted features. These models include but are not limited to:
- Logistic Regression
- Random Forest
- Gradient Boosting

### Evaluation

Models were evaluated based on various metrics such as accuracy, confusion matricies, and ROC-AUC scores. Cross-validation and hyperparameter tuning techniques were employed to optimize model performance. 
Below are the results of our baseline logistic regression model with no pre-preocessing or hyperparameter tuning.

![image](https://github.com/Gfatouras/Phase3/assets/165408353/fe1c998b-b7da-4c04-8abc-afcb1b3d710a)



Below are the results of our decision tree model using catboost for hyperparameter tuning.

![image](https://github.com/Gfatouras/Phase3/assets/165408353/569350b2-93a9-4af5-966f-a359423d0366)


## Conclusion

The project successfully demonstrates the feasibility of predicting vaccination behaviors using machine learning techniques. By leveraging data-driven insights, stakeholders can make informed decisions to improve vaccination strategies and public health outcomes.

For detailed implementation and results, refer to the project's codebase and documentation.
