# House Price Prediction
Predicting house prices using 79 variables. The dataset, obtained from Kaggle, contains 79 variables and 1640 entries. The target variable is the sale price.

## 1. Exploratory Data Analysis (EDA):
This phase includes an analysis of the target variable, examining normality, outliers, linearity, and homoscedasticity. For highly correlated numeric variables (continuous), a similar analysis is conducted, examining normality, outliers, linearity, and homoscedasticity. Categorical variables with high separating power are also analyzed.

## 2. Data Wrangling:
This step involves identifying null values and deciding whether to drop or impute them based on their correlation and the extent of nulls in the variable. The mode of imputation is determined by the variable. Flags are created for certain variables, and transformations are applied to adjust normality based on the EDA findings (using log, sqrt, and cbrt). Numeric columns are normalized, and categorical variables are subjected to one-hot encoding.

## 3. Simple Regression Models:
Various models, including CatBoost, XGBoost, LGBoost, RandomForest, and SVM, are used. The models are evaluated using RMSE, and further hyperparameter tuning is performed.

## 4. Hyperparameter Tuning:
RandomSearchCV and GridSearchCV are employed to find the best-fit parameters, with RMSE as the scoring metric for evaluation.

## 5. Stacking Model and Voting Model:
Stacking and voting models are built based on the results of the base models.

## 6. Neural Network:
A neural network with dropout is implemented.

## 7. Model Evaluation:
RMSE values of all models are compared, and CatBoost is selected based on the lowest RMSE.

## 8. Prediction on Test Set:
The best model, CatBoost, is used for predicting house prices on the test set obtained from Kaggle.

Note: Ensure that the variable names, model names, and details are accurate and consistent throughout the document. Adjust as needed based on your actual workflow and results.
