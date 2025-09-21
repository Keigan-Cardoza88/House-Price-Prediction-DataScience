**House Price Prediction**

A supervised machine learning, DataScience project, that predicts house prices using the Ames Housing dataset. The project covers data cleaning, preprocessing, exploratory data analysis, feature engineering, outlier handling, model training, hyperparameter tuning, and model evaluation.

**Project Overview**

The goal was to create a robust regression model to predict housing prices based on property characteristics such as lot size, location, construction details, and amenities.

Steps included:
1. Preprocessing the dataset by handling missing values and encoding categorical features.
2. Performing exploratory data analysis (EDA) to identify key price-driving factors.
3. Detecting and handling outliers for more stable model performance.
4. Feature scaling and transformation for better model convergence.
5. Training and comparing multiple ML algorithms.
6. Hyperparameter tuning to optimize model performance.


**Dataset & Features**

Dataset: Ames Housing Dataset
Target Variable: SalePrice
Example feature categories:
Numerical: LotArea, OverallQual, YearBuilt, GrLivArea, GarageCars
Categorical: Neighborhood, HouseStyle, Exterior1st, RoofStyle, SaleCondition

Steps Performed:
**Missing Value Handling**

1. Imputed numerical features with median values.
2. Imputed categorical features with mode.
3. Label Encoding & One-Hot Encoding
4. Applied label encoding for ordinal features.
5. Used one-hot encoding for nominal categorical features.

**Exploratory Data Analysis (EDA)**
1. Distribution plots for SalePrice (log-transformed).
2. Correlation heatmaps to identify highly predictive variables.
3. Boxplots & scatterplots for feature-price relationships.

**Outlier Detection & Handling**
1. Applied IQR method and visual inspection for outliers in LotArea, GrLivArea, etc.
2. Removed extreme anomalies to avoid skewed model learning.

**Feature Scaling**
1. Applied StandardScaler for models sensitive to scale (LR, Ridge, Lasso).
2. Checked log transformation for skewed features.

**Model Training & Evaluation**
1. Baseline model: Linear Regression

Models tested:
1. Linear Regression (LR)
2. Lasso Regression
3. Ridge Regression
4. Random Forest Regressor
5. Gradient Boosting Regressor
6. HistGradientBoosting Regressor
7. XGBoost Regressor

Evaluation Metrics:
R² Score
Root Mean Squared Error (RMSE)
Cross-validation scores

**Best model: Gradient Boosting**

**Hyperparameter Tuning**
1. Used GridSearchCV and RandomizedSearchCV to tune hyperparameters.
2. Optimal parameters improved model stability and reduced overfitting.

**Model Saving**
Final trained model saved using joblib for reuse.

📈 Results
Best model: Gradient Boosting Regressor
R² Score Tested: 0.91
RMSE: Significantly reduced after tuning; 0.108 

Robust generalization on unseen data

💻 Technologies Used
Python 3.11
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
XGBoost
Joblib

**How to Run**

1. Install Python (≥3.10) and Jupyter Notebook.
2. Download the .ipynb file within the repository.
3. Download the Ames Housing dataset and place it in the project folder.
4. Open the notebook/script(.ipynb) and run all cells.
5. The trained model (.pkl) will be generated.
6. Run the evaluation notebook to test predictions.

**The Model is also present within repository!!**

**© Copyright & Usage Disclaimer**

© 2025 Keigan Cardoza. All rights reserved.

This project represents my own work, including all code, analysis, and documentation, and is protected under applicable copyright laws.
The contents of this repository are not intended for public use, redistribution, or commercial purposes. They are provided solely for testing, demonstration, and educational review purposes.

By accessing or using any part of this repository, you acknowledge that:
1. You will not claim this work as your own or misrepresent its authorship.
2. You will not redistribute or commercially exploit any part of the code, datasets, or documentation without prior written permission from the author.
