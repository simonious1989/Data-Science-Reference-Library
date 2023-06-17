
### Contents
- [Definition](#definition)
- [Types of classification](#types-of-classification)
- [Feature Engineering Techniques](#feature-engineering-techniques)
- [Model Evaluation](#model-evaluation)
- [Classification Example](#classification-example)


### Definition




### Types of classification

- Simple linear regression: one independent variable
- Multiple linear regression: multiple independent variables
- Polynomial regression: a non-linear relationship between variables



### Feature Engineering Techniques

- [one]()
- [one]()
- [one]()
  

### Model Evaluation




### Regression Example

> Suppose we now build the model to predict whether a patient suffers from heart disease.
> Use train_test_split with a test_size of 0.2 and random_state set to 100. What is the test accuracy of our model?

```

import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score

# Load the data
data = pd.read_csv('heart.csv')

# Split the data into independent variables (X) and the target variable (y)
X = data.drop('target', axis=1)
y = data['target']

# Split the data into training and test sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=100)

# Create a Logistic Regression model and fit it to the training data
model = LogisticRegression()
model.fit(X_train, y_train)

# Make predictions on the test set
y_pred = model.predict(X_test)

# Calculate the test accuracy
test_accuracy = accuracy_score(y_test, y_pred)
test_accuracy

```
