# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import the required libraries such as Pandas and Scikit-learn to handle data and perform linear regression.
<br>

### Step2
Read the cars.csv file using Pandas and store it in a dataframe.
<br>

### Step3
Select Weight and Volume as independent variables (X) and CO2 as the dependent variable (y).
<br>

### Step4
Create a linear regression model and train it using the dataset with the fit() function.
<br>

### Step5
Then use the trained model to predict the CO2 emission and display the result.
<br>

## Program:
```
# Developed by: YASHVANDAN K
# Register No: 212225100060

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))

```
## Output:

<img width="1367" height="454" alt="image" src="https://github.com/user-attachments/assets/610ee2af-003a-46e0-8dfd-dbd13d4532c1" />

<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
