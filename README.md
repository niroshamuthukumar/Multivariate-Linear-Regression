# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas

### Step2
import linear model from sklean

### Step3
read the file cars.csv

### Step4
assign the values for x and y as required

### Step5
create the linearRegression model and predict the output

## Program:
```
#Developed by: Nirosha M
#Register Num: 23014438

import pandas as pd
from sklearn import linear_model
df=pd.read_csv('/content/cars.csv')
x=df[['weight','volume']]
y=df['CO2']
regr=linear_model.linearRegression()
regr.fit(x,y)
print("Coefficient:"regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("predicted CO2 for the corresponding weight and volume",predictedCO2)

```
## Output:
![Alt text](<Annotation 2023-12-27 213702.png>)
## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.