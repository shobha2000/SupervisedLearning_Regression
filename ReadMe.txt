In this implementation, we start by loading the "Medical Price Dataset.csv" file using pd.read_csv and storing it in the data DataFrame.

Next, we preprocess the data by extracting the features (age and BMI) and the target variable (charges) from the DataFrame and storing them in x_train and y_train, respectively.

Optionally, we normalize the features to ensure they are on a similar scale. This step can be skipped if the features are already normalized.

Then, we set the hyperparameters such as the learning rate and the number of iterations for the gradient descent algorithm.

The linear_regression function performs the gradient descent algorithm. It initializes the parameters, adds a column of ones to the features matrix for the intercept term, calculates the predicted values, calculates the cost, calculates the gradients, and updates the parameters iteratively.

After training the linear regression model using the linear_regression function, we print the coefficients (theta) and plot the cost history to visualize the convergence of the algorithm.