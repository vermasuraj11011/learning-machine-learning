## Random Forest Intuition

Random Forest is an ensemble learning method used for both classification and regression tasks. 
It builds multiple decision trees and merges their predictions to improve accuracy and reduce over-fitting.
Here's an intuition and a high-level definition of a Random Forest model:

### Intuition:

**Ensemble of Trees:** Random Forest builds a collection (ensemble) of decision trees 
during training.<br>
**Random Feature Selection:** At each node of a decision tree, instead of considering all
features, Random Forest randomly selects a subset of features for making decisions. 
This introduces diversity among the trees.<br>
**Bootstrap Aggregating (Bagging):** Each tree in the Random Forest is trained on a different 
subset of the training data. This is achieved through a process called bootstrapping, where
random samples with replacement are drawn from the training dataset.<br>
**Voting or Averaging:** For classification tasks, each tree "votes" for a class, and the class with the majority of votes becomes the final prediction. For regression tasks, the predictions of all trees are averaged.

### High-level Definition:
Random Forest is an ensemble learning method that constructs a multitude of decision trees during 
training and outputs the mode (for classification) or mean prediction (for regression) of the 
individual trees. The randomness introduced in feature selection and data sampling helps to 
decorrelate the trees, leading to a more robust and accurate model.

### Key Features:
**Decision Trees:** The base learners in a Random Forest are decision trees. These trees are 
typically shallow to avoid over-fitting.<br>
**Random Feature Subset:** At each node of a tree, a random subset of features is considered 
for splitting, reducing correlation between trees.<br>
**Bootstrapping:** Each tree is trained on a bootstrap sample (random sample with replacement)
from the original dataset.<br>
**Ensemble Averaging/Voting:** The final prediction is obtained by aggregating the predictions 
of all trees, either through voting (for classification) or averaging (for regression).<br>
**Robustness:** Random Forest is known for its robustness and ability to handle noisy and complex
datasets.

Random Forest is widely used in practice due to its versatility, ease of use, and ability to provide high-quality predictions across a variety of tasks. It is a powerful tool for both beginners and experienced practitioners in machine learning.

### See more 
- [Random Forest Regression](https://scikit-learn.org/stable/modules/ensemble.html#random-forests)
