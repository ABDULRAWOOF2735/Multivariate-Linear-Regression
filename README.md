# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1

import pandas library and linear_model from sklearn using import statement.
Step2

Read the given csv file using read_csv() method.
Step3

Create two arrays,independent array x with two classes and dependent array y with one class.find the regression of x and y using linear_model.LinearRegression() method and fit x and y using.fit()method.
Step4

Find the coefficients using .coef_and intercept using.intercept_
Step5

predict the linear regression using regr.predict()method and display the result
## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)


```
## Output:

### Insert your output
![Screenshot 2025-04-30 114733](https://github.com/user-attachments/assets/f21aef6d-da13-4382-81b1-edd056fb352b)

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
