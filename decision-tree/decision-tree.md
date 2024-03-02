## Decision Tree

A Decision Tree is a supervised machine learning algorithm used for both classification and 
regression tasks. It creates a model that predicts the target variable by learning simple 
decision rules inferred from the features of the data. Here's a definition and an overview 
of a Decision Tree model:

### Definition:

A Decision Tree is a hierarchical tree-like model consisting of nodes, where each node represents
a decision or a test on an attribute, each branch represents the outcome of the decision, and each 
leaf node represents the final predicted outcome (class label for classification or numerical value
for regression).

### Key Components:

**Root Node:** The topmost node in the tree, representing the feature that best splits the data based on certain criteria.
**Internal Nodes:** Nodes that represent decisions or tests on features. They lead to further nodes or leaves based on the outcome of the test.
**Branches:** Connections between nodes representing the possible outcomes of a decision.
**Leaves (Terminal Nodes):** Endpoints of the tree where the final prediction is made. In classification, each leaf corresponds to a class label, and in regression, it represents a numerical value.
**Splitting Criteria:** The criteria used to determine how to split the data at each internal node. Common criteria include Gini impurity for classification and mean squared error for regression.

### How a Decision Tree Works:
**Selection of Root Node:** The algorithm selects the feature that best separates the data based on a chosen criterion.
**Splitting Data:** The dataset is divided into subsets based on the values of the chosen feature at the root node.
**Recursive Splitting:** The process is repeated for each subset at the child nodes, creating a tree structure until a stopping condition is met.
**Stopping Conditions:** The tree-building process stops when a predefined depth is reached, or the number of instances in a node falls below a certain threshold.
**Predictions:** Once the tree is built, new data can be classified or predicted by traversing the tree from the root to a leaf node.

### Advantages of Decision Trees:
**Interpretability:** Decision Trees are easy to understand and interpret, making them suitable for explaining the reasoning behind predictions.
**Handle Non-Linearity:** They can model complex relationships between features and the target variable, including non-linear relationships.
**No Assumptions About Data Distribution:** Decision Trees do not make assumptions about the distribution of data.

Decision Trees are foundational in machine learning and serve as the building blocks for more advanced ensemble methods like Random Forests and Gradient Boosted Trees.



### See more 
- [Decision Tree](https://scikit-learn.org/stable/modules/tree.html#tree)