## Support Vector Regression (SVR) 
It is a type of regression algorithm that uses support vector machines (SVM) for regression analysis.
It is particularly useful for tasks where the relationship between the input variables and the output
variable is complex and non-linear.

Here's a brief overview of how SVR works:

- **Objective**: SVR aims to find a function that predicts the output variable (target) based on input features. The goal is to minimize the error of the predictions.
- **Kernel Trick**: SVR uses a kernel function to transform the input features into a higher-dimensional space. This allows SVR to capture complex relationships between variables that may not be apparent in the original feature space.
- **Margin of Tolerance**: SVR introduces a margin of tolerance around the predicted values. The model aims to fit the data within this margin, and any data points falling outside the margin contribute to the model's error.
- **Loss Function**: SVR uses a loss function that penalizes errors based on how far they are from the true values. The loss function includes a regularization term to prevent overfitting.
- **Hyperparameters**: SVR has hyperparameters like the choice of kernel, regularization parameter (C), and kernel-specific parameters. These need to be tuned to achieve the best model performance.
- **Prediction**: Once trained, the SVR model can make predictions on new, unseen data by transforming the input features using the learned kernel function.

It's important to note that SVR is effective in high-dimensional spaces and is especially useful when the relationship between variables is non-linear. However, proper tuning of hyperparameters is crucial for optimal performance. Additionally, SVR may not be suitable for large datasets due to its computational complexity.



### See more 
- [SVR](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html)