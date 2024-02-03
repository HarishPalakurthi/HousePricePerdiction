# HousePricePerdiction
House price prediction using 79 variables
The dataset is obtained from Kaggle and it contains 79 variables and 1640 entries.
For the prediction of saleprice (target variable). The following is the workflow.
# 1. Explporatory Data Analysis:
    It includes analysis of target variable: normality, outliers, linearity, homoscedasiticity
    Highly correlated numeric convariables (continuous) and their analysis : normality, outliers, linearity, homoscedasiticity
    Analysis on categorical variables (High Seperating Power)
# 2. Data Wrangling:
    It includes finding null values and based on their correlation and extent of nulls in the variable t; the decision on the variavle whether to     drop, impute will be taken also  mode of imputation bsed on the variable
    Creation of flags for certain variables
    Applying transformations to adjust normality etc from EDA (using log, sqrt and cbrt)
    Normalization of numeric columns and Onehot encoding for categorical variables
# 3. Simple regression models
    
