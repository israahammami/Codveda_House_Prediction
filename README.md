🏡 Boston Housing Price Prediction - End-to-End ML Pipeline

This project demonstrates an end-to-end Supervised Machine Learning pipeline built using Python and scikit-learn. The objective is to analyze historical real estate data and accurately predict median house prices based on various neighborhood features (such as crime rate, pupil-teacher ratio, and number of rooms).

📊 Project Workflow & Methodology
1* Data Ingestion & Audit:Loaded the classic 506-neighborhood dataset, assigned standard column names, and verified data integrity (no missing values).
2* Exploratory Data Analysis (EDA): Generated a correlation matrix to mathematically measure how every single feature relates to the others and to the target price (MEDV).
3* Data Partitioning: Isolated features ($X$) and targets ($y$), then partitioned the dataset into an 80% training set (404 houses) and a 20% hidden testing set (102 houses) to prevent data leakage and ensure fair model evaluation.
4* Model Training & Comparison: Trained and evaluated two distinct regression algorithms:Baseline Model: Linear Regression (straight-line mathematical rules).Advanced Model: Random Forest Regressor (ensemble of decision trees capturing non-linear pricing logic).

📈 Model Performance Results
The models were evaluated using two metrics on the 102 hidden test houses:
** RMSE (Root Mean Squared Error): Average prediction error in thousands of dollars (Lower is better).
** $R^2$ (R-squared): Proportion of variance explained (Higher is better).

🔍 Key Insights (Random Forest Feature Importance)
Extracting feature importance from the winning Random Forest model revealed that the top three drivers of house prices in this dataset are:

RM (Average number of rooms per dwelling) - Highly positive correlation with price.

LSTAT (Percentage of lower status population in the area) - Highly negative correlation with price.

PTRATIO (Pupil-teacher ratio by town) - Negative correlation.

🛠️ Tech Stack & Libraries
Language: Python

Core Libraries: pandas, numpy, matplotlib, scikit-learn

Model Serialization: joblib

Environment: Jupyter Notebook / VS Code
