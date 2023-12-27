# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas

### Step2
Import linear_model

### Step3
Read the csv file

### Step4
Enter the parameters to implement

### Step5
Run the program 

## Program:
```
'''
#Program to implement multivariate linear regression and predict the output.
#Developed by: GUTTHA KEERTHANA
#RegisterNumber: 212223240045
'''
import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars (1).csv")
X=df[['Weight','Volume']]
Y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(X,Y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)
```


## Output:
![](multi.png)
![](multi1.jpg)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
