![Polynomial_Regression](https://github.com/BaraSedih11/Polynomial-Regression/assets/98843912/62061da3-fb5f-4f90-9c35-d1ac2befa7ca)

Exercise: Polynomial Regression
Get some practice implementing polynomial regression in this exercise. In data.csv, you can see data generated for one predictor feature (Var_X) and one outcome feature (Var_Y), following a non-linear trend. Use sklearn's PolynomialFeatures(opens in a new tab) class to extend the predictor feature column into multiple columns with polynomial features. Play around with different degrees of polynomials to see what fits best!

Perform the following steps below:
1. Load in the data

The data is in the file called 'data.csv'. Note that this data has a header line.
Make sure that you've split out the data into the predictor feature in X and outcome feature in y.
For X, make sure it is in a 2-D array of 20 rows by 1 column. You might need to use NumPy's reshape(opens in a new tab) function to accomplish this.
2. Create polynomial features

Create an instance of sklearn's PolynomialFeatures(opens in a new tab) class and assign it to the variable poly_feat. Pay attention to how to set the degree of features, since that will be how the exercise is evaluated.
Create the polynomial features by using the PolynomialFeatures object's .fit_transform()(opens in a new tab) method. The "fit" side of the method considers how many features are needed in the output, and the "transform" side applies those considerations to the data provided to the method as an argument. Assign the new feature matrix to the X_poly variable.
3. Build a polynomial regression model

Create a polynomial regression model by combining sklearn's LinearRegression(opens in a new tab) class with the polynomial features. Assign the fit model to poly_model.
