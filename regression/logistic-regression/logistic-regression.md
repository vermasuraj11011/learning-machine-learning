# Logistic Regression

Logistic Regression is a statistical model that in its basic form uses a logistic function to model a binary dependent
variable, although many more complex extensions exist. In regression analysis, logistic regression (or logit regression)
is estimating the parameters of a logistic model (a form of binary regression).

## How Logistic Regression Works:

1. **Binary Logistic Regression:** The logistic regression model computes a weighted sum of the input features plus a
   bias term, but instead of outputting the result directly like the linear regression model does, it outputs the
   logistic of this result.

2. **Estimating Probabilities:** The logistic—also called the logit, noted σ(·)—is a sigmoid function (i.e., S-shaped)
   that outputs a number between 0 and 1. It is defined as follows: σ(t) = 1 / (1 + exp(-t)).

3. **Making Predictions:** Logistic Regression model prediction y = σ(θ^T · x) = hθ(x), where σ is the logistic function
   and θ^T · x is the dot product of the parameter vector θ and the instance vector x.

## Advantages of Logistic Regression:

- **Outputs have a nice probabilistic interpretation:** The logistic regression model can estimate the probability that
  an instance belongs to a particular class.

- **The algorithm can be regularized to avoid overfitting:** Logistic models can be updated easily with new data using
  stochastic gradient descent.

## Disadvantages of Logistic Regression:

- **Logistic regression tends to underperform when there are multiple or non-linear decision boundaries:** They are not
  flexible enough to naturally capture more complex relationships.

- **Not flexible enough to capture complex relationships:** Logistic regression will not perform well with independent
  variables that are not correlated to the target variable and are very similar or correlated to each other.

## Applications of Logistic Regression:

Logistic Regression is used in various fields, including machine learning, most medical fields, and social sciences. For
example, the Trauma and Injury Severity Score (TRISS), which is widely used to predict mortality in injured patients,
was originally developed by Boyd et al. using logistic regression.

Please note that this is a general overview of the Logistic Regression algorithm. Depending on the specifics of your
project, you might want to add more details or examples.