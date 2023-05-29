# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step 1: Import pandas as pd.
Step 2: From sklearn imort linear_model.
Step 3: Using Linear Regression stratergy calculate and fit the data.
Step 4: Using Scatter plot() scatter the x and y datas and find the best fit data.

## Program:
```
import pandas as pd

from sklearn import linear_model

df=pd.read_csv("/content/cars (1).csv")

x=df[['Weight','Volume']]

y=df['CO2']

regr=linear_model.LinearRegression()

regr.fit(x,y)

print("Coefficient:",regr.coef_)

print("Intercept:",regr.intercept_)

predictedCO2=regr.predict([[3300,1300]])

print("Predicted CO2 for the corresponding weight and volume",predictedCO2)
```
## Output:
![image](https://github.com/Meetha22003992/Multivariate-Linear-Regression/assets/119401038/cd4bed89-5664-4c2c-a88f-bbb2bd4a40b4)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
