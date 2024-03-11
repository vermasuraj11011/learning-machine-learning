# K-Nearest Neighbours

K-Nearest Neighbours (KNN) is a simple yet powerful machine learning algorithm used for classification and regression.
It stores all available cases and classifies new cases based on a similarity measure (e.g., distance functions). A new
record is classified by a majority vote of its neighbors, with the case being assigned to the class most common amongst
its K nearest neighbors measured by a distance function.

## How KNN Works:

1. **Store all available cases:** KNN starts by storing all the available data points (cases).

2. **Calculate Distance:** For a new data point, the distance from this point to all other points is calculated. The
   distance can be any type of measure and it depends on the type of data. Commonly used measures include Euclidean
   distance, Manhattan distance, and Minkowski distance.

3. **Find Closest Neighbors:** Identify the 'K' points in the training data that are nearest to the new data point.

4. **Vote for Labels:** The new data point is then assigned the label based on majority vote. For example, if K=3, and
   the three closest points to the new data point are 1 class A and 2 class B, then the new data point would be
   classified as class B.

## Advantages of KNN:

- **Simple to understand and explain:** The algorithm is straightforward and easy to explain.

- **No assumptions about data:** KNN makes no assumptions about the underlying data distribution. This is an advantage
  in cases where the data does not meet the assumptions of other algorithms.

- **Versatility:** KNN can be used for both classification and regression problems.

## Disadvantages of KNN:

- **Computationally expensive:** KNN can be computationally expensive as it stores all the training data.

- **Sensitive to irrelevant features:** The algorithm is sensitive to irrelevant features and the scale of the data.

- **Optimal number of neighbors:** Choosing the optimal number of neighbors (K) can be challenging.

## Applications of KNN:

KNN has a wide range of applications including economic forecasting, data compression, and genetics. For example, in
genetics, KNN can be used to identify the genetic markers that are associated with a particular disease.