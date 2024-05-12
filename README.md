# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and Y variables.

### Step4
Create the linear regression model and fit.

### Step5
Print the Coefficients and Intercept.

### Step6
Predict the CO2 emission of a car where the weight is 3300kg, and the volume is 1300cm3.

### Step7
Print the predicted output.

## Program:
```
'''
Program to implement multivariate linear regression.
Developed by: SANDHIYA R
RegisterNumber: 212223240146
'''
import pandas as pd
from sklearn import linear_model

data = pd.read_csv("cars.csv")

X = data[['Weight','Volume']]
Y = data['CO2']

regr = linear_model.LinearRegression()
regr.fit(X,Y)

print('Coefficients: ',regr.coef_)
print('Intercept: ',regr.intercept_)

predictCO2 = regr.predict([[3300,1300]])
print('Predicted CO2 for corresponding Weight and Volume',predictCO2)

```
## Output:

### Insert your output

![image](https://github.com/SandhiyaRajagopal/Multivariate-Linear-Regression/assets/144870852/41bc73e9-57be-4c6c-b334-b853b99f7d82)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
