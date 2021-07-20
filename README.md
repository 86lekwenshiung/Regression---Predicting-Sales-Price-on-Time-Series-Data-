# **Predicting Sales Price from Time Series Data**

## 1.0 Problem Statement
- How might we be able to predict the future sales price of a bulldozer , using the equipment features and previous data of sold bulldozer?

## 2.0 Datasets and Additional resources
- kaggle :  https://www.kaggle.com/c/bluebook-for-bulldozers/data
- udemy : Complete Machine Learning & Data Science Bootcamp 2021 by Daniel Bourke
- Train.csv : training set through end of 2011
- Valid.csv : validation set from Jan 2012 to Apr 2012
- Test.csv : May 2012 to Nov 2012

## 3.0 Data Dictionary
https://docs.google.com/spreadsheets/d/18ly-bLR8sbDJLITkWG7ozKm8l3RyieQ2Fpgix-beSYI/edit?usp=sharing

## 4.0 Approach to Problem Solving
We're going to take the following approach:
1. Problem definition
2. Data
    - FIllna numeric cell with median
    - Fillna non-numeric cell via conversion to pd.Categorical.codes
4. Evaluation
    - Main evaluator : RMSLE
    - Additional evaluator : R2 , MSE
6. Features
    - Explore feature importances via model inbuilt function feature_importances_
7. Modelling
    - Random Forest Regressor
8. Experimentation
    - Hyperparameter tuning with Randomized Search CV

## 5.0 Models used for exploration
- Random Forest

## 6.0 Conclusion
- After the model is built and evaluated with the test datasets, we like to learn which bulldozer sales attribute were the most important for predictings the overall sales price out of so many columns inputed. By performing a feature studies on the model, we will able to further focus ourstudies onto this parameters (YearMade , ProductSize , Enclsure , SaleYear , etc) in future work.
