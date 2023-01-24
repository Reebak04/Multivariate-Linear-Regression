# Implementation of Multivariate Linear Regression

## Aim

To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:

1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
3.	
## Algorithm:

### Step1

<br>import pandas as pd

### Step2

<br>Read the csv file

### Step3

<br>Get the value of x and y variables

### Step4

<br>Create the linear regression model and fit 

### Step5

<br>Predict the CO2 emission of a car where the weight is 2300kg,and the volume is 1300cm cube
 
### Step6

<br>Print the predicted output

## Program:
```
'''
developed by: Tejusve kabber.F`
reference.no: 22002543
'''
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("csvfile.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficients:",regr.coef_)
print("intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```
## Output:

### Insert your output

<br>![mvlr](https://user-images.githubusercontent.com/118364993/214362365-3e9126c9-dbc7-426e-b825-c9469ca75278.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
