# Linear-Kernel-for-Support-Vector-regression
Creating a linear kernel code for a Support Vector Regression Problem for a concrete data set.
Importing all thr libraies we need.
At first reading the data excel file using "pd.read_excel" and checking if there are any missing values if any then filling the missing values  by their column mean respectively.
furthermore normalizing the data importing "MinMaxScaler".
Seperateing input data X and y.
Spiliting the data into training and testing data set in the ratio of 8:2 respectively.
Defining a function for linear kernel for a support vector regressionand returing 4 types of error which helps us to decide the hyper-parameter values. Errors are calculating using sklearn library.
For chosing the hyperparameter we use k-fold cross validation and grid search(here I used 5-fold cross validation). In linear kernel our hyper-parameter C which is in range (2^(-10), 2^(10)). Getting the value of C for minimum MSE error.
Then applying the linear kernel for testing dataset using optimum hyperparameter C, and calculating MSE, RMSE, MAE, R2 error.

