# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import Pandas library.
### Step2
Import Linear_model from sklearn.
### Step3
Read the csv file using pandas library.
### Step4
Enter the parameters of the linear function.
### Step5
Print the parameters of the linear function.
## Program:
```
#NAME : MANIKANDAN K
#REG NO : 212224230150
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:\\Users\\admin\\Downloads\\car (1).csv")
df
x=df[['Volume','Weight']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficients:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted:",predictedCO2)

```
## Output:
<img width="717" height="112" alt="image" src="https://github.com/user-attachments/assets/be5fd118-187e-4ed3-bff4-6d7bf0d9f79f" />
<img width="363" height="850" alt="image" src="https://github.com/user-attachments/assets/8d8b38df-007e-43ae-a4a9-fe150e42aae2" />
<img width="807" height="371" alt="image" src="https://github.com/user-attachments/assets/8f93adb2-6c0c-4a71-9659-8b919cd5e86d" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
