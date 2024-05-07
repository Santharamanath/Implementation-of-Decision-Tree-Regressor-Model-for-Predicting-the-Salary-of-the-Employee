# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the standard libraries.

2.Upload the dataset and check for any null values using .isnull() function.

3.Import LabelEncoder and encode the dataset.

4.Import DecisionTreeRegressor from sklearn and apply the model on the dataset.

5.Predict the values of arrays.

6.Import metrics from sklearn and calculate the MSE and R2 of the model on the dataset.

7.Pedict the values of array.

8.Apply to new unknown values.
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Santha ramanath M

RegisterNumber:212223220097

import pandas as pd
data=pd.read_csv("Salary.csv")

data.head()

data.info()

data.isnull().sum()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data["Position"]=le.fit_transform(data["Position"])
data.head()

x=data[["Position","Level"]]
x.head()

y=data[["Salary"]]

from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test=train_test_split(x,y,test_size=0.2,random_state=2)

from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)


from sklearn import metrics
mse=metrics.mean_squared_error(y_test, y_pred)
mse

r2=metrics.r2_score(y_test,y_pred)
r2

dt.predict([[5,6]])  
*/
```

## Output:
![322170999-7c004e33-9234-49da-a096-4e369a05df3c](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/c197e8b1-ff34-4708-bb64-be47b3af902c)

![322171009-5c5645e6-d814-4f0b-aa28-c0c2479f7b7d](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/a949f6dd-d95d-4283-94e7-a8b9b821b836)


![322171019-38714279-17aa-4abe-a762-74d66f047252](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/a671b746-2c21-404b-a109-792a0ba034c6)

![322171028-ab7af8cf-0006-48bc-ac68-017abfa92525](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/5fe7b3f5-19f7-4861-a6f2-ba9e34a2de78)

![322171046-2cb7ad3a-817d-450e-90e7-628f99c117d1](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/ccdf6fb7-6f83-4f48-a385-694b0ed9efb2)

![322171056-d947b775-a9ab-41e4-8be7-b439aeb3c1f8](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/1e4d5b79-9fe6-400c-b788-a30b56f45377)

![322171075-78ac948c-dc27-4a82-81f1-0f777e7871aa](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/3ebfb29d-a9db-4ca3-8795-c71e97d44555)


![322171086-6d45c9fa-fb44-44da-b92d-bc80724bfdd9](https://github.com/Santharamanath/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/149035289/af872091-e325-492a-8fda-f4f90b0ef248)



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
