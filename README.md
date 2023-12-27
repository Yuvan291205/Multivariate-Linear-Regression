# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pands module to solve for multivariate linear regression

### Step2
from sklearn import linear_model

### Step3
open the file cars saved in the drive and get input for weight and volume to find density of CO2

### Step4
print coefficients,intercept and amount

### Step5
end of the program

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv('/content/drive/MyDrive/cars (1).csv')
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
![Screenshot 2023-12-27 085146](https://github.com/Yuvan291205/Multivariate-Linear-Regression/assets/138849170/37759806-d24c-4326-a8f5-72fa8606d35b)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
