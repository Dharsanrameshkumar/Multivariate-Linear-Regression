# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Step1:
 andas as pdImpport.

Step2:
Read the csv file.

Step3:
Get the value of X and y variables.

Step4:
Createar regression model and fit.
 the line
Step5:
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.

Step6:
Print the predicted output.


### Step1
<br>Import pandas as pd

### Step2
<br>Read the csv file.

### Step3
<br>Get the value of X and y variables

### Step4
<br>Create the linear regression model and fit.

### Step5
<br>Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3.



## Program:
```
#Developed by: Dharsan
#Register number: 212223100003

import pandas as pd
from sklearn import linear_model

df=pd.read_csv('/content/cars (1).csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient",regr.coef_)
print("Intercept",regr.intercept_)
print("Amount",regr.predict([[3300,1300]]))


```
## Output:
![Alt text](ex10.jpg)
### Insert your output

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.