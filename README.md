# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary packages using import statement. 2.Read the given csv file and print the number of contents to be displayed. 3.Split the dataset using train_test_split. 4.Calculate Y_Pred and accuracy. 5.Display the result.

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: HARSSHITHA LAKSHMANAN
RegisterNumber: 212223230075

import numpy as np
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.feature_extraction.text import CountVectorizer
from sklearn import svm
from sklearn.metrics import classification_report, accuracy_score
df= pd.read_csv('/content/spam.csv', encoding='ISO-8859-1')
df.head()
vectorizer= CountVectorizer()
x= vectorizer.fit_transform(df['v2'])
y=df['v1']
x_train, x_test, y_train, y_test= train_test_split(x,y,test_size=0.25, random_state=42)
model= svm.SVC(kernel='linear')
model.fit(x_train, y_train)
predictions= model.predict(x_test)
print("Accuracy:", accuracy_score(y_test, predictions))
print("Classification Report:")
print(classification_report(y_test, predictions)) 
*/
```

## Output:
![SVM For Spam Mail Detection](sam.png)
![image](https://github.com/harshulaxman/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145686689/efd3d431-4618-4d1a-ba20-6ddf5a3b40a0)
![image](https://github.com/harshulaxman/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145686689/3ca97d0b-37a2-4ac9-aef4-04afc3f57ee8)
![image](https://github.com/harshulaxman/Implementation-of-SVM-For-Spam-Mail-Detection/assets/145686689/c86e56cc-64a2-4a6d-9750-db7656d6d8e1)


## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.
