# Diabetes Prediction using Machine Learning

## Project Overview

This project predicts whether a patient is diabetic based on medical attributes such as Glucose, BMI, Blood Pressure, Insulin, Age, and Pregnancy history.

The project includes data preprocessing, exploratory data analysis (EDA), feature scaling, model training, hyperparameter tuning, and model comparison using Logistic Regression and Random Forest.

## Dataset

- Records: 768
- Features: 8
- Target Variable: Outcome
  - 0 = Non-Diabetic
  - 1 = Diabetic

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

## Data Preprocessing

- Checked missing values
- Replaced medically invalid zero values using Median Imputation
- Performed Exploratory Data Analysis
- Applied StandardScaler for feature scaling

## Exploratory Data Analysis

Key observations:

- Glucose showed the strongest relationship with diabetes.
- BMI and Age were important predictors.
- Insulin contained significant outliers.
- Several features exhibited positive skewness.

## Models Used

### Logistic Regression

Best Parameters:

- C = 1
- Solver = liblinear

Results:

- Test Accuracy: 75.0%
- Cross Validation Accuracy: 76.88%

### Random Forest

Best Parameters:

- n_estimators = 100
- max_depth = None
- min_samples_split = 2

Results:

- Test Accuracy: 73.38%
- Cross Validation Accuracy: 77.85%
- ROC-AUC Score: 0.834

## Feature Importance

Top predictors identified by both models:

1. Glucose
2. BMI
3. Age
4. DiabetesPedigreeFunction

## Model Comparison

| Model | Accuracy | CV Score | ROC-AUC |
|---------|---------|---------|---------|
| Logistic Regression | 75.0% | 76.88% | 0.822 |
| Random Forest | 73.38% | 77.85% | 0.834 |

## Conclusion

Logistic Regression achieved the highest test accuracy and provided good interpretability. Random Forest achieved a higher ROC-AUC score, indicating stronger discrimination between diabetic and non-diabetic patients across different classification thresholds.

Glucose, BMI, and Age were identified as the most important predictors of diabetes.


## Author

Albin Karintholil Robert

MSc Data Science and Analytics
