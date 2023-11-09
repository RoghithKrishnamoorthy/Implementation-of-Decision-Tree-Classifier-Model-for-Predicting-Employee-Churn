# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. import the required libraries.

2. Upload and read the dataset.

3. Check for any null values using the isnull() function.

4. From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.

5. Find the accuracy of the model and predict the required values by importing the required
module from sklearn.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: ROGHITH K
RegisterNumber:  212222040135
import pandas as pd
data=pd.read_csv("/content/Employee.csv")

print('data.info:')
data.info()

print('data.isnull().sum():')
data.isnull().sum()

print('value_count: ')
data["left"].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()

data["salary"]=le.fit_transform(data["salary"])
data.head()

*x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()**

y=data["left"]

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)

from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy

dt.predict([[0.5,0.8,9,260,6,0,1,2]])
*/
```

## Output:
![ex 6 1.Initial data set](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/0ef8ec83-74a0-43df-ac7e-0843ab7c57af)
![ex 6 2.Data Info](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/683507f4-f0bb-45e8-a9af-42f3dbe3a888)
![ex 6 3.Optimization of null values](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/867a47ae-d9d3-4869-82b4-0c144649c461)
![ex 6 4.Values count in Left coloumn](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/a9482d82-1765-4fb9-9e2b-75d6896c8f15)
![ex 6 5.DataSet Transformed Head](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/6db4cc25-f3ed-4028-858c-e616def07a92)
![ex 6 6.x.head](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/c342e574-6515-4f11-a419-0121b18d4ec8)
![ex 6 7.Accuracy](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/a84aee81-6144-4247-82ac-8e03eb3ff89a)
![ex 6 8.Data Prediction](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/22ee253f-0b6f-4033-a5bd-76a1f87e1ee0)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
