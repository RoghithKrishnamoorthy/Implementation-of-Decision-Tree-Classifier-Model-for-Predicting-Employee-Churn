# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

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

## Output:![Screenshot 2023-10-12 093638](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/0f85023d-76c1-416d-be80-70c7c603693b)
![Screenshot 2023-10-12 094436](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/40a8b885-c239-4677-a1c7-3e482060c834)
![Screenshot 2023-10-12 093941](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/771b2e45-d4ac-4f8e-8c61-8293fb9b3bfa)
![Screenshot 2023-10-12 094032](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/e8ee6e54-9b0e-4df6-a78d-9fde9b196068)
![Screenshot 2023-10-12 094128](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/0585143a-3326-4aa7-8d17-ef3a21c041bd)
![Screenshot 2023-10-12 094324](https://github.com/RoghithKrishnamoorthy/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119475474/5d8e5828-928c-4c41-b202-35f04e11cd01)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
