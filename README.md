# Healthcare-Cost-Prediction-using-Machine-Learning
Machine learning project to predict healthcare costs using patient demographic and lifestyle factors, with data preprocessing, exploratory data analysis, and regression model evaluation.

##  Project Overview

This project uses machine learning techniques to predict healthcare costs based on patient demographic, lifestyle, and health-related factors.

The project focuses on understanding the factors that influence healthcare expenses and comparing different regression models to identify the model that provides better prediction performance.

##  Project Objective

The main objectives of this project are to:

* Predict individual healthcare costs using patient information.
* Explore relationships between patient characteristics and healthcare charges.
* Identify the key factors influencing healthcare costs.
* Compare Linear Regression and Random Forest Regression models.
* Evaluate model performance using appropriate regression metrics.

##  Dataset

The dataset contains information about patients and their healthcare costs.

Key features include:

Age– Patient's age
Sex – Patient's gender
BMI – Body Mass Index
Children – Number of children/dependants
Smoker – Smoking status
Region – Patient's residential region
Charges – Healthcare cost / medical charges

The target variable is:

Charges

 Exploratory Data Analysis

Exploratory Data Analysis (EDA) was performed to understand the dataset and identify relationships between the variables.

The analysis included:

* Checking data types and dataset structure
* Identifying missing values
* Checking duplicate records
* Examining descriptive statistics
* Analysing numerical and categorical variables
* Exploring correlations between variables
* Visualising relationships between important features and healthcare charges

A correlation heatmap was used to identify relationships between numerical variables.

## Data Preprocessing

The following preprocessing steps were performed:

1. Checked for missing values.
2. Checked and removed duplicate records.
3. Handled missing values using forward filling where required.
4. Encoded categorical variables into numerical values.
5. Separated the independent variables (`X`) from the target variable (`y`).
6. Split the dataset into training and testing sets using an 80/20 split.
7. Applied feature scaling using `StandardScaler`.

The data was split into training and testing sets **before scaling** to prevent data leakage. The scaler was fitted only on the training data and then used to transform the test data.

## Machine Learning Models

Two regression models were developed and compared.

### 1. Linear Regression

Linear Regression was used as a baseline model to understand the relationship between the input variables and healthcare charges.

### 2. Random Forest Regression

Random Forest Regression was used to capture more complex and non-linear relationships between patient characteristics and healthcare costs.

The model was configured using multiple decision trees to improve prediction performance and reduce the limitations of a single decision tree.

 Model Evaluation

The models were evaluated using the following metrics:

### Mean Absolute Error (MAE)

MAE measures the average absolute difference between the actual and predicted healthcare costs.

**Lower MAE = better performance**

### Root Mean Squared Error (RMSE)

RMSE measures the square root of the average squared prediction errors. It gives greater weight to larger errors.

**Lower RMSE = better performance**

### R² Score

R² measures how much of the variation in healthcare costs is explained by the model.

**Higher R² = better performance**

 Model Comparison

The performance of Linear Regression and Random Forest Regression was compared using MAE, RMSE and R².

Based on the evaluation results, **Random Forest Regression performed better than Linear Regression** for this dataset.

This indicates that the relationship between patient characteristics and healthcare costs may include non-linear patterns that Random Forest was able to capture more effectively.

 Feature Importance

Feature importance from the Random Forest model was analysed to identify the variables that contributed most to healthcare cost predictions.

The analysis indicated that important factors included:

Smoking status
BMI
Age
These variables showed a strong influence on predicted healthcare costs.
Programming Language

* Python

Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

 Machine Learning

* Linear Regression
* Random Forest Regression
* Train/Test Split
* StandardScaler
* Model Evaluation

 Key Findings
The project provided the following key insights:

* Healthcare costs vary considerably between patients.
* Smoking status has a significant relationship with healthcare costs.
* BMI is an important factor associated with healthcare expenses.
* Age also contributes to differences in healthcare costs.
* Random Forest Regression provided better predictive performance than Linear Regression.
* Feature importance analysis helped identify the major factors influencing healthcare cost predictions.



