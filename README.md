# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start the program.
2. Import the python pandas library as pd.
3. Read the contents of the Spam csv file.
4. Display the first 5 rows of the dataset using head().
5. Assign x as v1 values and y as v2 values.
6. From sklearn library select the feature extraction and import CountVectorizer.
7. CountVectorizer will convert the Text to Numerical Data.
8. From sklearn library import Support Vector Classifier (ie. SVC).
9. Predict the x_test using SVC.
10. Print the accuracy of the SVM Model 11.Stop the program.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: JEEVITHA S
RegisterNumber:212222100016

import chardet
file='/content/spam.csv'
with open(file, 'rb') as rawdata:
  result = chardet.detect(rawdata.read(100000))
result

import pandas as pd
data=pd.read_csv("/content/spam.csv",encoding = 'Windows-1252')

data.head()

data.info()

data.isnull().sum()

x=data["v1"].values

y=data["v2"].values

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=0)

from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()

x_train=cv.fit_transform(x_train)
x_test=cv.transform(x_test)

from sklearn.svm import SVC
svc=SVC()
svc.fit(x_train,y_train)
y_pred=svc.predict(x_test)
y_pred

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
*/
```

## Output:
### Result output:
![242841614-f02335b4-97d3-4a67-9748-cdc639fd40d4](https://github.com/Jeevithha/Implementation-of-SVM-For-Spam-Mail-Detection/assets/123623197/531072fd-1b41-4f23-a772-1c49449463b7)
### data.head():
![242841732-3d99a04d-f230-44d8-a8be-6c255a566833](https://github.com/Jeevithha/Implementation-of-SVM-For-Spam-Mail-Detection/assets/123623197/8371228c-d7b6-4d48-990c-8272333a2639)
### data.info():
![242841857-900fc1b4-5dd7-44d8-afa6-01f8c71cfab4](https://github.com/Jeevithha/Implementation-of-SVM-For-Spam-Mail-Detection/assets/123623197/7b2f7cbb-95de-4321-98c1-b7e1d606f9fe)
### data.isnull().sum():
![242841940-109c8db0-556b-42d9-a19a-888628ec281e](https://github.com/Jeevithha/Implementation-of-SVM-For-Spam-Mail-Detection/assets/123623197/e3b7dbc0-975c-4a74-90e0-c732a55303e5)
### Y_Prediction value:
![242842047-42966bc4-a936-49cb-b495-ea2a7ec8905e](https://github.com/Jeevithha/Implementation-of-SVM-For-Spam-Mail-Detection/assets/123623197/e7928039-8e22-4a76-908c-29d5389b9916)
### Accuracy value:
![242842215-5a427e7d-f05e-4656-8d23-9523ca01711e](https://github.com/Jeevithha/Implementation-of-SVM-For-Spam-Mail-Detection/assets/123623197/ac3d359e-8bf8-4104-9c5e-c941bb36f8a1)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
