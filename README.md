# Regression Models: Boston Housing Data

## Data
The data being used for regression modeling is the Boston Housing Dataset from the MASS package in R. This data consists of 506 observations and 14 variables. The resultant variable to be predicted is “medv”, i.e. the median value of owner-occupied homes in $1000s. This resultant variable is present in the 14th column of the dataset.

## Goal and Background
The objective of this analysis is to fit different predictive models onto the training and testing subsets of the dataset and evaluate the in-sample and out-of-sample performance of each model. The following models’ performances are compared: <br>
•	General Linear Model <br>
•	Tree model - CART <br>
•	Advanced Tree Models - Bagging, Random Forest, Boosting <br>
•	Generalized Additive Model <br>
•	Neural Network <br>

## Approach
We begin the analysis by an initial exploratory data analysis to get a preliminary understanding of the relationships among the different variables. The data is then split into 70% training data set and 30% testing data set. For linear regression model, we select variables using backward elimination with AIC as criterion, and for all the other models we assume a full model. Finally, we calculate and compare the different models’ performances - the metrics used to assess the training and testing errors are MSE and MSPE respectively. 

## Findings
<table>
  <tr><td>Model <td> MSE <td>  MSPE </tr>
  <tr><td>General Linear Model <td> 17.49 <td>  33.8 </tr>
  <tr><td>Regression Tree <td> 13.1 <td>  29.83 </tr>
  <tr><td>Bagging <td> 10.44 <td>  23.48 </tr>
  <tr><td>Random Forest <td> 2.02 <td>  14.05 </tr>
  <tr><td>Bosting <td> 0.03 <td>  14.28 </tr>
  <tr><td>Generalized Additive Model <td> 6.12 <td>  18.26 </tr>
  <tr><td>Neural Network <td> 4.13 <td>  16.11 </tr>
</table>  
The ideal predictive model for this data set is the Boosting algorithm.
