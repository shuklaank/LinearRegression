# Linear Regression Implementation with Regularization

This repository contains a Python implementation of Linear Regression with two methods: Closed Form and Gradient Descent. It also includes feature engineering, regularization using L2 (Ridge Regression), and options to use gradient descent or stochastic gradient descent. Additionally, it provides a plotting function to visualize the cost during training. 

## Methods for Linear Regression

### A. Closed Form
- Check for low rank matrices
- Check for full rank matrices
- Handle different dataset sizes

### B. Gradient Descent
- Initialize theta
- Define the loss function (J(theta))
- Find the derivative

## Feature Engineering
- Add an intercept column of 1 to the feature matrix
- Normalize data (normalize training data and apply the same normalization to test data)
- Split the dataset into training and test sets

## Input and Hyperparameters
- Input data: X, y
- Hyperparameters: 
  - Alpha (learning rate)
  - Max Iterations
  - Epsilon (tolerance for error)

## Regularization
Add L2 (Ridge Regression) regularization to:
   - Normal equation (Closed form solution)
   - Gradient Descent

Pass the regularization parameter as an option to the `LinearRegression` class to enable or disable regularization.

## Stochastic Gradient Descent
- Added a function to calculate Stochastic Gradient Descent and pass necessary parameters to the class to switch between gradient descent and stochastic gradient descent.

## Error Visualization
- Included a plotting function to visualize the cost during the training steps.

## Testing and Reporting
- Verified the functions using test datasets and the provided information in the documentation.

## Reporting Results
- Calculated and reported Root Mean Squared Error (RMSE) and Sum of Squared Errors (SSE) over the test set for all three datasets.

## Observations
- The choice of learning rate affects the convergence speed. A larger learning rate can lead to faster convergence but may overshoot the minimum, while a smaller learning rate may converge more slowly but steadily.

- The regularization parameter controls the trade-off between fitting the training data and preventing overfitting. A larger regularization parameter will result in a simpler model with smaller coefficients, reducing overfitting.
