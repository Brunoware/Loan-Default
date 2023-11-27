# Credit Risk Modeling

## Overview

This repository contains Python code for credit risk modeling using logistic regression. The primary focus is on calculating the Probability of Default (PD), a key metric in assessing credit risk. The project compares traditional coefficient estimation using logistic regression with confidence interval calculation through regularization methods (Ridge, Lasso, ElasticNet).

## Introduction

Credit risk is the threat that a borrower may fail to meet financial obligations, stemming from either an inability or unwillingness to repay. Probability of Default (PD) represents the likelihood of payment default, aiding in binary classification of default and non-default values. Beyond classification, PD extends to predicting when default might occur, enabling banks to assess client profitability and implement risk management strategies.

The International Accounting Standards Board (IASB) established standards in the International Financial Reporting Standard 9 (IFRS 9) to guide entities in presenting relevant and useful information. Compliance with IFRS 9 enables banks to develop effective financial management practices and provide transparent information to stakeholders.

The project addresses the need for PD calculation in future periods, crucial for effective credit management. Two approaches are explored: using transition matrices from rating agencies and creating statistical models based on historical PDs from bank databases. While complex machine learning models offer superior performance, their lack of interpretability and potential overfitting pose challenges.

Hence, the project aims to develop a machine learning model with high interpretability and low complexity for PD calculation, striking a balance between efficacy and simplicity. The comparative analysis includes traditional logistic regression and regularization methods (Ridge, Lasso, ElasticNet), emphasizing mathematical perspectives.

## Code Structure

### 1. Preprocessing
- **1.1 Data Loading:** Importing necessary libraries and reading the dataset.
- **1.2 Data Preprocessing:** Handling data types, checking for missing values, and removing outliers.

### 2. Modeling
- **2.1 Dataset Division:** Splitting the dataset into feature matrix (X) and target variable (y).
- **2.2 Outliers Removal:** Using a custom function clean_outliers.
- **2.3 Imputation and Encoding:** Null value imputation and one-hot encoding of categorical features using ColumnTransformer.
- **2.4 Logistic Regression:** Fitting the logistic regression model with different penalties (none, L2, L1, ElasticNet).
- **2.5 Bootstrap Method:** Calculating confidence intervals of coefficients.
- **2.6 Model Evaluation:** Assessing the model using accuracy, recall, precision, F1 score, and ROC AUC.

### 3. Verification of Assumptions
- **3.1 Assumption Checks:** Verifying logistic regression assumptions, including target variable distribution, independence of observations, absence of multicollinearity, linearity of log odds, and sample size.

### 4. Use Case
- **4.1 Scenario Analysis:** Calculating Expected Credit Loss (ECL) under different scenarios (base, optimistic, pessimistic, normal).
- **4.2 Quantiling Probabilities:** Assigning probabilities to quantiles.
- **4.3 ECL Calculation:** Calculating Expected Credit Loss and presenting results.

## Results

Visualizations and tables present results, including coefficient confidence intervals, assumption verification plots, and ECL calculations.

## How to Use

1. Clone the repository using `git clone`.
2. Install required Python libraries with `pip install -r requirements.txt`.
3. Execute the Jupyter notebook or Python script.

Feel free to customize the code for your dataset or use case.

## License

This code is released under the [MIT License](LICENSE).

## Authors

- Bruno Miranda
- Jorge Fernandez