# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee


## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
Step 1. Data Collection
Step 2. Data Preprocessing
Step 3. Model Training
Step 4. Model Evaluation
Step 5. Prediction

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Meyyappan T
RegisterNumber:  212223240086
*/

import pandas as pd
data = pd.read_csv("./Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data['Position'] = le.fit_transform(data['Position'])
data.head()
x = data[['Position','Level']]
y = data[['Salary']]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size = 0.2,random_state = 2)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_predict)
mse
r2=metrics.r2_score(y_test,y_predict)
r2
dt.predict([[5,6]])
```
### Output:
![image](https://github.com/arbasil05/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/144218037/6919eca6-d510-49bb-9881-5fe5d3d504b5)
![image](https://github.com/arbasil05/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/144218037/eddd0d7f-744f-431c-8d35-03917e9ee404)
![image](https://github.com/arbasil05/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/144218037/d9717383-87aa-45f9-b34e-9c8787f7667f)
![image](https://github.com/arbasil05/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/144218037/e570f14e-a2b2-4612-ab0f-0a3a02b71964)
![image](https://github.com/arbasil05/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/144218037/c303810d-5cec-400b-b239-ce22d9281b9c)
![image](https://github.com/arbasil05/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/144218037/c8d5f779-f07d-42a0-b554-db0b4aff609e)
![image](https://github.com/arbasil05/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/144218037/69ddae50-b0b9-48a4-8d87-00847601fcb7)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
