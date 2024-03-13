# Random Forest Classification:

Random Forest is a supervised learning algorithm that uses multiple decision trees to solve classification and
regression problems. It operates by constructing several decision trees at training time and outputting the class that
is the mode of the classes (classification) or mean prediction (regression) of the individual trees.

1. **Creating Subsets of Dataset:** The algorithm starts by creating multiple subsets of the original dataset. This is
   done by randomly selecting samples from the dataset with replacement (bootstrap samples).

2. **Building Decision Trees:** For each subset, a decision tree is built. During the construction of the tree, only a
   random subset of features are considered for splitting a node. This randomness helps to make the model more robust
   and less prone to overfitting.

3. **Making Predictions:** When making predictions, each tree in the Random Forest gives its own prediction and the
   final prediction is made by taking the majority vote for classification, or an average for regression.

## Advantages of Random Forest:

- **Handling Overfitting:** Random Forest reduces overfitting problem in decision trees and also reduces the variance
  and therefore improves the accuracy.
- **Handling Large Datasets:** It can handle large datasets with high dimensionality.
- **Estimating Missing Data:** Random Forest can maintain accuracy when a large proportion of the data are missing.

## Disadvantages of Random Forest:

- **Complexity:** Random Forest creates a lot of trees and combines their outputs. By default, it creates 100 trees in
  Python sklearn library. To do so, this algorithm requires much computational power and resources.
- **Longer Training Period:** Random Forest require much more time to train as compared to decision trees as it
  generates a lot of trees and makes decision on the majority of votes.

## Decision Tree:

A Decision Tree is a supervised machine learning algorithm used for both classification and regression tasks. It creates
a model that predicts the target variable by learning simple decision rules inferred from the features of the data.

- **Root Node:** The topmost node in the tree, representing the feature that best splits the data based on certain
  criteria.
- **Internal Nodes:** Nodes that represent decisions or tests on features. They lead to further nodes or leaves based on
  the outcome of the test.
- **Branches:** Connections between nodes representing the possible outcomes of a decision.
- **Leaves (Terminal Nodes):** Endpoints of the tree where the final prediction is made. In classification, each leaf
  corresponds to a class label, and in regression, it represents a numerical value.
- **Splitting Criteria:** The criteria used to determine how to split the data at each internal node. Common criteria
  include Gini impurity for classification and mean squared error for regression.

## Advantages of Decision Trees:

- **Interpretability:** Decision Trees are easy to understand and interpret, making them suitable for explaining the
  reasoning behind predictions.
- **Handle Non-Linearity:** They can model complex relationships between features and the target variable, including
  non-linear relationships.
- **No Assumptions About Data Distribution:** Decision Trees do not make assumptions about the distribution of data.

Decision Trees are foundational in machine learning and serve as the building blocks for more advanced ensemble methods
like Random Forests and Gradient Boosted Trees.