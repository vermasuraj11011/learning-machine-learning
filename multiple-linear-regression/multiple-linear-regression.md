## Multiple Linear Regression

Multiple Linear Regression (MLR) is a statistical method used for modeling 
the relationship between a dependent variable and multiple independent 
variables. It extends the concept of simple linear regression, where there 
is only one predictor variable.

In MLR, the relationship between the dependent variable (also known as the
response variable) and two or more independent variables is modeled as a 
linear equation. The general form of the equation for MLR with 'p' 
independent variables is:

````text
Y = β0 + β1 * X1 + β2 * X2 + ... +  βp * Xp + ε
````

Y is the dependent variable.    
X1, X2, ... Xp are the independent variables.   
β0 is the intercept (constant term).    
β1 ,β2 , .. ,βp are the coefficients representing the strength and direction of the relationships.  
ε is the error term, representing the unobserved factors that affect the dependent variable 
but are not included in the model.

The goal of MLR is to estimate the coefficients (β values) in a way that minimizes the sum of 
squared differences between the observed and predicted values. This is typically done using a
method like Ordinary Least Squares (OLS).

MLR assumes that the relationships between the variables are linear, and the model's accuracy 
is evaluated based on how well it fits the observed data. It is a powerful tool in statistics 
and machine learning for predicting and understanding the relationships between multiple variables.