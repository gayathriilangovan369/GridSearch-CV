# Insurance Charges Prediction

In this project, I worked on predicting medical insurance charges using machine learning. The goal was to understand how factors like age, BMI, smoking habits, and number of children influence insurance costs.

## Overview

I built and compared multiple regression models to estimate insurance charges. The workflow includes data preprocessing, encoding categorical variables, training models, and improving performance using GridSearchCV.

## Dataset

The dataset includes demographic and health-related information such as age, sex, BMI, number of children, and smoking status.

Features used:
- Age  
- Sex  
- BMI  
- Children  
- Smoker  

Target:
- Charges  

## Data Preparation

- Converted categorical variables like sex and smoker using One-Hot Encoding  
- Cleaned and prepared the dataset  
- Applied scaling where needed (especially for SVR)  

## Models

- Support Vector Regression (SVR)  
- Decision Tree Regressor  
- Random Forest Regressor  

## Model Tuning

Used GridSearchCV with cross-validation to find the best parameters for each model.

## Understanding GridSearchCV

Initially, hyperparameter tuning was done manually by trying different parameter combinations, which was time-consuming and less efficient.

GridSearchCV automates this process by testing multiple parameter combinations using cross-validation and selecting the best one based on model performance.

This makes the tuning process faster, more structured, and more reliable.

## Results

Model performance based on R² score:

- SVR: 0.85989  
- Random Forest: 0.85166  
- Decision Tree: 0.69556  

SVR achieved the highest R² score, while Random Forest also performed well and provided stable predictions.

## Key Observations

- Smoking status has a strong impact on insurance charges  
- BMI and age also influence the cost  
- Ensemble models like Random Forest provide consistent performance  

## Tools Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  

## How to Run

Open the Jupyter notebooks and run the cells step by step.

## Final Thoughts

This project helped me understand how different machine learning models perform on real data and how tuning improves results. It also gave useful insights into the main factors affecting insurance costs.
