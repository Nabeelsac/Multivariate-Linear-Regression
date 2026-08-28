# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
Import Pandas and the required module from Scikit-learn.
Read the carsemission.csv dataset.
Select Weight and Volume as independent variables.
Select CO2 as the dependent variable.
Create and train a Multivariate Linear Regression model.
Display the regression coefficients and intercept.
Predict the CO₂ emission for:
Weight = 3300
Volume = 1300
Display the predicted CO₂ emission.
## Program:
```
import pandas as pd
from sklearn import linear_model
df = pd.read_csv("carsemission.csv")
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
Coefficients: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted CO2 for the corresponding weight and volume: [114.75968007]

### Insert your output
<img width="701" height="80" alt="image" src="https://github.com/user-attachments/assets/339a0c22-4137-450e-9d70-088a53321507" />


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
