
## R-squared

R-squared (coefficient of determination) is a statistical measure that represents the proportion
of the variance in the dependent variable that is predictable from the independent variables.
It provides an indication of how well the independent variables explain the variability of the
dependent variable in a regression model. R-squared is a common metric used for evaluating the
performance of regression models.

### overview of R-squared:

- **Range:** R-squared values range from 0 to 1. A value of 0 indicates that the model does not explain any variance in
  the dependent variable, while a value of 1 indicates that the model perfectly explains the variance.
- **Interpretation:** An R-squared value close to 1 suggests that a high proportion of the variability in the dependent
  variable is captured by the independent variables in the model. On the other hand, a low R-squared value indicates
  that the model does not effectively explain the variability.
- **Calculation:** R-squared is calculated as the proportion of the sum of squared differences between the predicted
  values and the mean of the dependent variable (total sum of squares) to the sum of squared differences between the
  observed values and the mean of the dependent variable (residual sum of squares).

````text
R^2 = Residual Sum of Squares / Total Sum of Squares
````

- **Limitations:** R-squared should be used with caution, as it has some limitations. For example, it can be
  artificially inflated by adding more independent variables to the model, even if they are not meaningful predictors.
  Additionally, a high R-squared does not necessarily imply causation.

In summary, R-squared provides a measure of how well the independent variables explain the variability in the dependent
variable. It is commonly used for model evaluation, but it is important to consider other metrics and the context of the
specific problem when assessing the overall performance of a regression model.

## Adjusted R-Square

The adjusted R-squared is a modified version of the R-squared (coefficient of determination) that accounts for the
number of predictors or independent variables in a regression model. While R-squared measures the proportion of variance
in the dependent variable explained by the independent variables, adjusted R-squared adjusts this value to penalize the
inclusion of unnecessary variables that do not significantly contribute to the explanation of variance.

The formula for adjusted R-squared is:

````text
Adjusted R^2 = (1 − (1 - R^2) * (n - 1)) / (n - k - 1)

where:
n is the number of observations.
k is the number of independent variables.
````

The adjusted R-squared takes into account the number of predictors in the model and penalizes models that include
additional variables without improving the overall explanatory power. Unlike R-squared, the adjusted R-squared can
decrease if the inclusion of a new variable does not sufficiently improve the model.

### Key points about adjusted R-squared:

- **Range:** Similar to R-squared, the adjusted R-squared value ranges from 0 to 1. A higher value indicates a better
  fit, but it considers the complexity of the model.
- **Interpretation:** A higher adjusted R-squared suggests that a larger proportion of the variability in the dependent
  variable is explained by the independent variables, considering the number of predictors.
- **Comparison:** When comparing models with different numbers of predictors, the adjusted R-squared is often preferred
  over R-squared.
- **Consideration:** While adjusted R-squared helps address the issue of overfitting, it should be used in conjunction
  with other model evaluation metrics, and the choice of predictors should be based on theoretical and practical
  considerations.

In summary, adjusted R-squared provides a more realistic measure of the goodness of fit by adjusting for the number of
predictors in a regression model. It is particularly useful when comparing models with different complexities to avoid
over-fitting.


### See more 
- [sk-learn r-score](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.r2_score.html#sklearn.metrics.r2_score)

