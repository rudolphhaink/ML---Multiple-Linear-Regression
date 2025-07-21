# Student Performance Multiple Linear Regression Analysis

## Overview

This project demonstrates a multiple linear regression analysis on the [Student Performance Dataset](https://archive.ics.uci.edu/ml/datasets/Student+Performance) to predict students’ final grades (`G3`) based on various demographic, academic, and social factors.

The project showcases:

- Data preprocessing, including handling categorical variables via dummy encoding
- Feature selection and train-test split
- Model training and evaluation (RMSE and R²)
- Diagnostic checks for multicollinearity, residual normality, and homoscedasticity
- Interpretation of regression coefficients and model metrics

---

## Dataset

The dataset contains student attributes such as demographics, study habits, family background, and previous grades. It is publicly available from the UCI Machine Learning Repository. The CSV file used here employs semicolon (`;`) as the delimiter.

---

## Project Structure

- `student_mat.csv`: Dataset file
- `student_performance_regression.ipynb`: Jupyter Notebook with code, analysis, and markdown explanations
- `README.md`: This file

---

## Key Findings

- The multiple linear regression model explains approximately **75% of the variance** in students' final grades, with an R² of **0.75**.
- The model's RMSE is about **2.26**, indicating the average prediction error in final grade points.
- **Previous grades (`G1` and `G2`)** are the strongest positive predictors of the final grade (`G3`).
- Students receiving **school support** tend to have higher final grades, as indicated by a positive coefficient.
- Participation in **extracurricular activities** and being in a **romantic relationship** are negatively associated with final grades.
- Having **higher education aspirations** shows a positive effect on final grades.
- Other positive influences include family relationship quality (`famrel`), male gender (`sex_M`), and having a mother who is a teacher (`mjob_is_teacher`).
- Variables such as **failures**, **alcohol consumption**, and **internet access** show small but significant negative effects.
- Multicollinearity is low to moderate with all **Variance Inflation Factors (VIFs) below 5**, indicating predictors are not highly correlated.
- Residuals from the regression are approximately **normally distributed**, satisfying an important assumption.
- The **Breusch-Pagan test indicates heteroscedasticity** (non-constant variance of residuals), suggesting potential issues with error variance that may require robust standard errors or model adjustments.

---

## 👤 Author

Rudolph Haink  
[LinkedIn](https://www.linkedin.com/in/rudolph-haink-a5454564/)
