# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
##Step1 Import the required Python libraries such as Pandas, NumPy, and Scikit-learn. Load the dataset using Pandas and display the first few rows to understand the data.

##Step2 Separate the independent variables (features) and the dependent variable (target) from the dataset.

##Step3 Split the dataset into training data and testing data using train-test split.

##Step4 Create a Multivariate Linear Regression model using the LinearRegression class. Train the model using the training dataset,use the trained model to predict the output values for the test dataset.

##Step5 Evaluate the performance of the model by comparing predicted values with actual values. Display the prediction results and interpret the output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("cars.csv")
X = df[['Weight', 'Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X, y)
print('Coefficients:', regr.coef_)
print('Intercept:', regr.intercept_)
input_data = pd.DataFrame({'Weight': [3300], 'Volume': [1300]})
predictedCO2 = regr.predict(input_data)
print('Predicted CO2 for the corresponding weight and volume:', predictedCO2)

```
## Output:

### Insert your output

<br><img width="1767" height="748" alt="Screenshot 2026-03-20 161631" src="https://github.com/user-attachments/assets/ea7f128d-d9c9-4ff4-be9e-d5e13fbe6d46" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
