
### Contents
- [Definition](#definition)
- [Types of regression](#types-of-regression)
- [Feature Engineering Techniques](#feature-engineering-techniques)
- [Model Evaluation](#model-evaluation)
- [Regression Example](#regression-example)


### Definition


Regression is a supervised learning algorithm that predicts continuous output values based on input data. 
For example you may want to predict the price of a car based on its make, model, year, and mileage. You would use regression to do this.


### Types of regression

- Simple linear regression: one independent variable
- Multiple linear regression: multiple independent variables
- Polynomial regression: a non-linear relationship between variables



### Feature Engineering Techniques

- [Scaling and Normalization](#scaling-and-normalization)
- Handling Missing Values
- Encoding Categorical Variables
- Feature Selection
- Feature Extraction
- Creating New Features

#### Scaling and Normalization
```
Required Package(s)
from sklearn.preprocessing import StandardScaler
```

```
# create scaler
scaler = StandardScaler()

# fit and transform data
X_scaled = scaler.fit_transform(X)
```

### Model Evaluation




### Regression Example

