# Regression Models: Boston Housing Data

## Data
The data being used for regression modeling is the Boston Housing Dataset from the MASS package in R. This data consists of 506 observations and 14 variables. The resultant variable to be predicted is “medv”, i.e. the median value of owner-occupied homes in $1000s. This resultant variable is present in the 14th column of the dataset.

## Goal and Background
The objective of this analysis is to fit different predictive models onto the training and testing subsets of the dataset and evaluate the in-sample and out-of-sample performance of each model. The following models’ performances are compared:
•	General Linear Model
•	Tree model - CART
•	Advanced Tree Models - Bagging, Random Forest, Boosting
•	Generalized Additive Model
•	Neural Network

## Approach
We begin the analysis by an initial exploratory data analysis to get a preliminary understanding of the relationships among the different variables. The data is then split into 70% training data set and 30% testing data set (seed is set to 13480226 to facilitate reproducibility). For linear regression model, we select variables using backward elimination with AIC as criterion, and for all the other models we assume a full model. Finally, we calculate and compare the different models’ performances - the metrics used to assess the training and testing errors are MSE and MSPE respectively. 

## Findings
Model   MSE   MSPE
General Linear Model    17.49   33.8
Regression Tree   13.1    29.83
Bagging   10.44   23.48
Random Forest   2.02    14.05
Boosting    0.03    14.28
Generalized Additive Model    6.12    18.26
Neural Network    4.13    16.11

The ideal predictive model for this data set is the Boosting algorithm.
