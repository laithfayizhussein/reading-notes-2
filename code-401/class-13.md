# Linear Regression in Python :
## How to run Linear regression in Python

- Linear regression : is one of the fundamental statistical and machine learning techniques. Whether you want to do statistics, machine learning, or scientific computing, there are good chances that you’ll need it. It’s advisable to learn it first and then proceed towards more complex methods.
- Regression analysis : is one of the most important fields in statistics and machine learning. There are many regression methods available. Linear regression is one of them.
- Regression searches for relationships among variables.
- When Do You Need Regression?
    to answer whether and how some phenomenon influences the other or how several variables are related
    is also useful when you want to forecast a response using a new set of predictors.
    Regression is used in many different fields: economy, computer science, social sciences, and so on
- Linear regression is probably one of the most important and widely used regression techniques. It’s among the simplest regression methods. One of its main advantages is the ease of interpreting results.

- The package scikit-learn : is a widely used Python library for machine learning, built on top of NumPy and some other packages. It provides the means for preprocessing data, reducing dimensionality, implementing regression, classification, clustering, and more. Like NumPy, scikit-learn is also open source.
- There are several ways in which you can do that, you can do linear regression using NumPy, scipy, stats model and sckit learn.
- Scikit-learn is a powerful Python module for machine learning. It contains functions for regression, classification, clustering, model selection and dimensionality reduction.
- sklearn.linear_model module : which contains “methods intended for regression in which the target value is expected to be a linear combination of the input variables”.
- steps to begin working :
    - import the required Python libraries into Ipython Notebook.
    - import data set into Ipython notebook and store it in a variable
    - convert data into a pandas data frame

## Exploring Boston Housing Data Set

- The first step is to import the required Python libraries into Ipython Notebook.

- This data set is available in sklearn Python module, so I will access it using scikitlearn. I am going to  import Boston data set into Ipython notebook and store it in a variable called boston.

- The object boston is a dictionary, so you can explore the keys of this dictionary.

## Scikit Learn

- In this section I am going to fit a linear regression model and predict the Boston housing prices. I will use the least squares method as the way to estimate the coefficients.

- Y = boston housing price(also called “target” data in Python)


- X = all the other features (or independent variables)

- First, I am going to import linear regression from sci-kit learn module. Then I am going to drop the price column as I want only the parameters as my X values. I am going to store linear regression object in a variable called lm.

## Apply the model for predictions.

- Types(cases) of the linear ewgression :

    - Multiple Linear Regression With scikit-learn

    - Polynomial Regression With scikit-learn

    - Advanced Linear Regression With statsmodels

- Linear regression is sometimes not appropriate, especially for non-linear models of high complexity.
- we use NumPy for handling arrays.
- Linear regression is implemented with the following:

    - scikit-learn : if you don’t need detailed results and want to use the approach consistent with other regression techniques
    - statsmodels : if you need the advanced statistical parameters of a model


