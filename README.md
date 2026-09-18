# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Import the required libraries such as pandas and LinearRegression.
2. Read the dataset from the CSV file and store it in a dataframe.
3. Select the input features (Volume, Weight) and output variable (CO2).
4. Create and train the Linear Regression model using the training data.
5. Display the coefficient, intercept, and predict the CO2 emission for the given input values [3300,1300].
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