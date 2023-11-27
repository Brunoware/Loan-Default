# Credit Risk Modeling

## Overview

This repository contains Python code for credit risk modeling using logistic regression. The code covers data preprocessing, model training with different regularization techniques (none, L2, L1, ElasticNet), and evaluation of the model. Additionally, the repository provides a use case scenario where Expected Credit Loss (ECL) is calculated under different scenarios.

## Code Structure

- **Preprocessing:** The initial section of the code focuses on importing necessary libraries, reading the dataset, and performing data preprocessing. This includes handling data types, checking for missing values, and removing outliers.

- **Modeling:** The second part involves model training and evaluation. It includes the following steps:
  - Division of the dataset into feature matrix (X) and target variable (y).
  - Outliers removal using a custom function `clean_outliers`.
  - Imputation of null values and one-hot encoding of categorical features using `ColumnTransformer`.
  - Fitting the logistic regression model with different penalties (none, L2, L1, ElasticNet).
  - Bootstrap method for calculating confidence intervals of coefficients.
  - Evaluation of the model using metrics such as accuracy, recall, precision, F1 score, and ROC AUC.

- **Verification of Assumptions:** This section checks various assumptions related to the logistic regression model, such as the distribution of the target variable, independence of observations, absence of multicollinearity, linearity of log odds, and the sample size.

- **Use Case:** The final part provides a practical use case scenario where Expected Credit Loss (ECL) is calculated under different scenarios (base, optimistic, pessimistic, and normal). This involves quantiling the output probabilities, calculating ECL, and presenting the results.

## Results

The code produces visualizations and tables to help interpret the results. Confidence intervals for coefficients, assumptions verification plots, and ECL calculations are presented in a clear and organized manner.

## How to Use

To run the code, follow these steps:

1. Ensure you have Python installed on your machine.
2. Clone this repository using `git clone`.
3. Install the required Python libraries by running `pip install -r requirements.txt`.
4. Execute the Jupyter notebook or Python script.

Feel free to customize the code for your specific dataset or use case.

## License

This code is released under the [MIT License](LICENSE).

## Author
[Bruno Miranda]
[Jorge Fernandez]
---


