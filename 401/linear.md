

# How to Run Linear Regression in Python :

In this quick post, I wanted to share a method with which you can perform linear as well as multiple linear regression, in literally 6 lines of Python code.
Check out the video version of this post if you prefer that !
[video How to Run Linear Regression in Python](https://youtu.be/X3ek_HIkZcQ)

In statistics, linear regression is a linear approach to modelling the relationship between a dependent variable and one or more independent variables. I you would like to know more about linear regression and how it is implemented, check out these two methods to perform Linear Regression from scratch:
![img](https://i.ibb.co/dKLjTkz/Screenshot-1.png)
[link](https://towardsdatascience.com/linear-regression-using-gradient-descent-97a6c8700931)

Today to perform Linear Regression quickly, we will be using the library scikit-learn. If you don’t have it already you can install it using pip:
```
pip install scikit-learn

```

So now lets start by making a few imports:

```
import numpy as np
import matplotlib.pyplot as plt  # To visualize
import pandas as pd  # To read data
from sklearn.linear_model import LinearRegression

```
We need numpy to perform calculations, pandas to import the data set which is in csv format in this case and matplotlib to visualize our data and regression line. We will use the LinearRegression class to perform the linear regression.

Now lets perform the regression:

```
data = pd.read_csv('data.csv')  # load data set
X = data.iloc[:, 0].values.reshape(-1, 1)  # values converts it into a numpy array
Y = data.iloc[:, 1].values.reshape(-1, 1)  # -1 means that calculate the dimension of rows, but have 1 column
linear_regressor = LinearRegression()  # create object for the class
linear_regressor.fit(X, Y)  # perform linear regression
Y_pred = linear_regressor.predict(X)  # make predictions
```

We have our predictions in Y_pred. Now lets visualize the data set and the regression line:

```
plt.scatter(X, Y)
plt.plot(X, Y_pred, color='red')
plt.show()
```
![img](https://miro.medium.com/max/378/1*Jat3oq1ZkuGvZsnL57JOmQ.png)
That’s it! You can use any data set of you choice, and even perform Multiple Linear Regression (more than one independent variable) using the LinearRegression class in sklearn.linear_model. Also this class uses the ordinary Least Squares method to perform this regression. So accuracy wont be high, when compared to other techniques. But if you want to make some quick predictions and get some insight into the data set given to you, then this is a very handy tool.

##### *Support or Contact:*

Having trouble with Pages? Check out our : [email](obada7jaber7@gmail.com) or phone number : 0781912474 or [contact support for gethub](https://support.github.com/contact) and we’ll help you sort it out. &#x1F691; &#x1F691; &#x1F691;
