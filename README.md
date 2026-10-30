# Implementation-of-Simple-Linear-Regression-Model-for-Predicting-the-Marks-Scored

## AIM:
To write a program to predict the marks scored by a student using the simple linear regression model.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Start
2. Import the required libraries (NumPy, Matplotlib and Scikit-learn).
3. Create a dataset containing hours studied and marks scored.
4. Separate the input (X) and output (Y) variables.
5. Split the dataset into training and testing data.
6. Create a Simple Linear Regression model.
7. Train the model using the training data.
8. Predict the marks using the trained model.
9. Display the predicted marks.
10. Plot the actual data points and regression line.
11. Display the graph.
12. Stop

## Program:
```
import numpy as np
import matplotlib.pyplot as plt
from sklearn.linear_model import LinearRegression

hours = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]).reshape(-1, 1)
marks = np.array([10, 20, 30, 40, 50, 60, 70, 80, 90, 100])

model = LinearRegression()

model.fit(hours, marks)

predicted_marks = model.predict(hours)

new_hours = np.array([[7.5]])
prediction = model.predict(new_hours)

print("Simple Linear Regression Model")
print("--------------------------------")
print("Slope:", model.coef_[0])
print("Intercept:", model.intercept_)
print("Predicted marks for 7.5 hours of study:", prediction[0])

plt.scatter(hours, marks, color='blue', label='Actual Marks')
plt.plot(hours, predicted_marks, color='red', label='Regression Line')

plt.xlabel("Hours Studied")
plt.ylabel("Marks Scored")
plt.title("Simple Linear Regression")
plt.legend()
plt.show()
```
/*
Program to implement the simple linear regression model for predicting the marks scored.
Developed by: SACHIN S.B
RegisterNumber: 212225040353
*/


## Output:
![simple linear regression model for predicting the marks scored](sam.png)
<img width="1531" height="782" alt="image" src="https://github.com/user-attachments/assets/4ba13269-072e-4e6d-bd2a-94e337a80675" />



## Result:
Thus the program to implement the simple linear regression model for predicting the marks scored is written and verified using python programming.
