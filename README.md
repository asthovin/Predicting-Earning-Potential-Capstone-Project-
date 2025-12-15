# Predicting-Earning-Potential-Capstone-Project-
Income Prediction and Exploratory Data Analysis (Adult Census Dataset)

This project focuses on analyzing factors that influence earning potential and predicting whether an individual earns more than 50K per year using the Adult Census dataset. The analysis includes data cleaning, statistical testing, visualization, and machine learning modeling.

Dataset

The dataset used in this project is the Adult Census Income dataset, commonly known as the “adult.data” file.

Source: UCI Machine Learning Repository (widely used public dataset)(Springboard Infosys)
File used: adult.data

The dataset contains demographic and employment-related information such as age, education, workclass, occupation, working hours, and income category.

Project Objective

The main objectives of this project are:

To understand the relationship between demographic features and income

To identify key factors influencing earning potential

To build a classification model to predict whether income exceeds 50K

Data Loading and Cleaning

The dataset is loaded without headers and column names are assigned manually. Missing values represented by “?” are handled by removing affected rows. String columns are cleaned by trimming extra spaces, and numeric columns are properly type-casted.

Outlier Handling

Outliers are handled using a combination of:

Domain-based constraints (for age and weekly working hours)

Interquartile Range (IQR) method for numerical features such as education years and capital values

Feature Selection and Transformation

Irrelevant or less useful columns are dropped to simplify analysis.
Income is converted into a binary target variable:

1 for income greater than 50K

0 for income less than or equal to 50K

Categorical variables are label encoded before modeling.

Exploratory Data Analysis

Several analyses and visualizations are performed, including:

Boxplots comparing weekly working hours across income groups

Correlation heatmap for numeric features

Line plots showing education level versus probability of high income

Scatter plot of age versus income category

Chi-square tests and Cramér’s V to measure association between categorical features and income

Bar charts showing probability of earning more than 50K by category

Statistical Tests

The project uses:

Independent t-tests to compare means between income groups

Chi-square tests of independence for categorical variables

Cramér’s V to measure strength of categorical associations

Modeling Approach

A Logistic Regression model is used for income classification. The dataset is split into training and testing sets. Model performance is evaluated using accuracy, precision, recall, F1 score, and a detailed classification report.

Feature Importance

Model coefficients from Logistic Regression are analyzed to understand the impact of each feature on income prediction. Weekly working hours and education years are highlighted as influential predictors.

Conclusion

This project provides a complete pipeline from raw data to insights and predictive modeling. It demonstrates practical data preprocessing, statistical analysis, and machine learning techniques commonly used in real-world data analysis tasks. The work can be further extended by trying different models, feature engineering techniques, or deploying the solution as an application.
