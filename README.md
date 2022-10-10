# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd. 

### Step2
Read the CSV file.

### Step3
Get the value of x and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.

### Step6
Print the predicted output.

## Program:
```python
## Developed by : yuvabharathi.b
## REGISTER NUMBER : 22002787

import pandas as pd
from sklearn import linear_model

data=pd.read_csv("cars.csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictCO2)
```

## Output:
![Screenshot from 2022-10-10 13-59-20](https://user-images.githubusercontent.com/113497404/194826047-ca2e96fe-b007-438c-bc4c-d1feacd98c04.png)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
