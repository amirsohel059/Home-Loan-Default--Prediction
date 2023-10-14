# Home Loan Default Prediction

This repository contains the code and documentation for a Home Loan Default Prediction project. The goal of this project is to predict whether a borrower will default on a home loan. It involves the analysis of various factors such as borrower characteristics, loan details, credit history, and other relevant features. The dataset used for this project is the `application_train.csv` file, which contains the target variable (1 for Defaulter and 0 for Not Defaulter).

## Table of Contents
- [Problem Statement](#problem-statement)
- [Libraries Used](#libraries-used)
- [Domain Analysis](#domain-analysis)
- [Exploratory Data Analysis](#exploratory-data-analysis)
  - [Univariate Analysis](#univariate-analysis)
  - [Bivariate Analysis](#bivariate-analysis)
  - [Income Band Analysis](#income-band-analysis)
- [Data Preprocessing](#data-preprocessing)
- [Features Selection](#features-selection)
- [Model Comparison Report](#model-comparison-report)
- [Report on Home Loan Default Prediction Dataset](#report-on-home-loan-default-prediction-dataset)
- [How to Contribute](#how-to-contribute)
- [How to Use](#how-to-use)
- [License](#license)

## Problem Statement

The project can be divided into the following tasks:

### Task 1: Data Analysis
- Prepare a comprehensive data analysis report on the given dataset.

### Task 2: Predictive Modeling
- Create a predictive model to identify the factors and customer segments that are eligible for taking a home loan.
- Compare the performance of multiple models on this dataset and recommend the best model for production use.

## Libraries Used

The following Python libraries are used in this project:
- `warnings`: To suppress warnings.
- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `seaborn`: For data visualization.
- `sweetviz`: For generating data analysis reports.
- `matplotlib`: For creating plots and charts.
- `scikit-learn`: For data preprocessing and machine learning models.
- `xgboost`: For the XGBoost Classifier.

## Domain Analysis

The dataset contains various features related to borrowers and their loan applications. Some of the key columns include `SK_ID_CURR` (unique identifier for each individual), `TARGET` (the target variable indicating loan repayment status), and various other columns describing borrower characteristics, financial details, and more.

## Exploratory Data Analysis

The exploratory data analysis includes both univariate and bivariate analyses. Some key insights are:

### Univariate Analysis
- The dataset is imbalanced with a higher number of clients repaying loans compared to those defaulting.
- There are more cash loan types than revolving loan contracts.
- Most people don't own cars, and those who do, have cars aged between 0-20 years.
- About 69% of people own real estate.
- Many people have no children, yet more than 60% are married.
- Most people have a normal working income and secondary-level education.
- The majority live in a house or apartment.
- Nearly all have mobile phones, but around 90% don't have email.
- There are a high number of people without all the required documents.

### Bivariate Analysis
- Cash loans are more likely to default compared to revolving loans.
- Although there are more females, more loans are defaulted by males.
- Marital status and education level play a significant role in loan default.
- Occupation and organization type also have an impact on loan default.
- Mismatched permanent addresses contribute to a higher rate of loan default.

### Income Band Analysis
There is little difference in income between those repaying and those defaulting on loans.

## Data Preprocessing

Data preprocessing involves addressing various challenges, including handling outliers, imputing missing values, addressing class imbalance, and managing correlated variables.

## Features Selection

Feature selection techniques were applied to choose the most informative variables for the models.

## Model Comparison Report

Based on the accuracy of the models, the XGBoost Classifier has the highest accuracy of 0.919, followed closely by the Random Forest Classifier with an accuracy of 0.917. XGBoost is recommended as the best model for production due to its strong performance and effectiveness in handling complex datasets.

## Report on Home Loan Default Prediction Dataset

This section provides a summary of the dataset, including its focus, challenges faced, techniques used, and reasoning behind various data preprocessing steps. The primary goal is to ensure the dataset is well-prepared for accurate predictions of home loan default.

For more details, please refer to the code and documentation in this repository.

## How to Contribute

If you would like to contribute to this project, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes to your fork.
5. Submit a pull request to the main repository.

## How to Use

To use this project, follow these steps:
1. Clone the repository to your local machine.
2. Install the required libraries as mentioned in the code.
3. Run the code and explore the data analysis and predictive modeling.

## License

This project is licensed under the [MIT License](LICENSE).
