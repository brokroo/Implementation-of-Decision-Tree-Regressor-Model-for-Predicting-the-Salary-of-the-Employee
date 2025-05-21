# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas

2.Import Decision tree classifier

3.Fit the data in the model

4.Find the accuracy score

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: SANJITH R 
RegisterNumber: 212223230191
import pandas as pd
data=pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
print(data.head())
x=data[["Position","Level"]]
print(x.head())
y=data["Salary"]
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
print(y_pred)
from sklearn import metrics
r2=metrics.r2_score(y_test,y_pred)
print(r2)
dt.predict([[5,6]])
*/
```

## Output:
![image](https://github.com/user-attachments/assets/f2f232c1-4bed-4ebd-8e84-931ddc5304c8)
![image](https://github.com/user-attachments/assets/6d8ea77b-029e-494f-8532-44bc1fb51c1d)
![image](https://github.com/user-attachments/assets/12c878e3-9253-438d-a308-cdbe4f31faa3)

![image](https://github.com/user-attachments/assets/fde59533-ad50-46e4-a5b7-62983b11b640)

![image](https://github.com/user-attachments/assets/a365fb43-60bc-4175-ba24-a7a2182bee38)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
