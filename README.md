Question 1>
The current implementation uses a fixed number of epochs (epochs=1000) as the convergence criterion. The gradient descent algorithm iterates for the specified number of epochs, regardless of whether the model has converged.

To improve the convergence criterion, we can implement an early stopping mechanism based on the change in the loss function (Mean Squared Error). For example, we could stop the training if the change in MSE between consecutive iterations falls below a small threshold.
Question 2>
Advantage of Averaging the Cost

Scaler independence: averaging ensures the cost function is independent of the dataset size. without averaging the cost would grow with number data pts.

Simplified learning rate: averaging keeps the gradient value in range, which helps in tuning the learning rate and ensures stability during gradient descent.

Numerical stability: averaging prevents the cost and gradient from becoming large, which could lead to numberical instability during computation.
