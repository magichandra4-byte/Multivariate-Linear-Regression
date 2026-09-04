# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Import the required libraries and dataset: Load libraries such as Pandas, NumPy, and Scikit-learn, then read the dataset containing multiple independent variables and one dependent variable.
2. Prepare the data: Separate the independent variables (features) from the dependent variable (target). Split the dataset into training and testing sets for model development and evaluation.
3. Create and train the model: Initialize the Multivariate Linear Regression model and train it using the training data. The model learns the relationship between multiple input variables and the target value.
4. Make predictions: Use the trained regression model to predict the target values for the testing data. Compare the predicted values with the actual values to check the model's performance.
5. Evaluate the model: Calculate evaluation measures such as Mean Squared Error (MSE) and R² score to determine the accuracy of the regression model. Display the results and analyze the relationship between the input variables and the predicted output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regression = linear_model.LinearRegression()
regression.fit(X, y)
print(regression.coef_)
print(regression.intercept_)
print("Predicted value:",regression.predict([[3300,1300]]))
```
## Output:

### Insert your output
![alt text](<ex 10.jpeg>)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.