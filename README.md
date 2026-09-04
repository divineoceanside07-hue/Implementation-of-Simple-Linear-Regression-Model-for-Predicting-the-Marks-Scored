# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import necessary libraries and create the dataset (X and Y).

2.Reshape the input data into a 2D format.

3.Create and train the Linear Regression model.

4.Obtain slope and intercept from the model.

5.Take user input and predict the output value.

6.Plot the actual data and regression line, then display the graph.
## Program:


Program to implement the simple linear regression model for predicting the marks scored.
Developed by: SRI RAM M
RegisterNumber:  212225040423
```
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

X = np.array([1, 2, 3, 4, 5]).reshape(-1, 1)
Y = np.array([35, 50, 65, 70, 85])
model = LinearRegression()
model.fit(X, Y)

x_input = float(input("Enter hours studied: "))
predicted_marks = model.predict([[x_input]])
print("Predicted Marks:", predicted_marks[0])
Y_pred = model.predict(X)
plt.scatter(X, Y, label="Actual Data")
plt.plot(X, Y_pred, label="Regression Line")
plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression (Using sklearn)")
plt.legend()
plt.show()
```

## Output:
<img width="837" height="609" alt="image" src="https://github.com/user-attachments/assets/884b661e-a462-41a4-a18b-b2bacb084130" />

## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
