# boston-city-crime-rate-prediction
This short project fits a simple and multiple linear regression on Boston city crime data and draws a comparison between the two results on statistically significant predictors for per capita crime rate. It also 

## Method
- The data consists of 500 observations with per capita crime rate in Boston as response variables and 13 predictors.
- Fitted a simple linear regression indiviually for each predictor on per capita crime rate.
- Fitted a multiple linear regression for all predictors together on per capita crime rate.
- For each method, beta coefficients, standard error, and p-value were calculated to measure the association of each predictor with the response variable.
- Looked for evidence of non-linear association between the predictors, age and tax (using their quadratic and cubic terms),  and the response crime rate. 

## Tools
Python, Jupyter Notebook, pandas, numpy, matplotlib, statsmodel

## Results
### Simple Linear Regression
- All the predictors except for 'chas' (represents tracts binding the river)  have statistically significant relationship with the response.
- 'Nox' representing nitric oxide concentration has a large positive association with the per capita crime rate.
- The predictor 'rm' representing average number of rooms per dwelling has a negative small association with the crime rate per capita.
- The predictor 'dis' representing weighted distance to Boston employment centers has a negative small association with the crime rate per capita.
- 'Medv' denoting median home value has a negative small association with the crime rate per capita.
- Though the coefficients are unstandardized, only nox seems to have a large association with the crime rate.
- All other predictors seem to have a smaller association with the crime rate.
### Multiple Linear Regression
- Proportion of residential land zoned for lots ('zn'), average number of rooms per dwelling ('rm'), proportion of owner-occupied units built prior to 1940 ('age'), index of accessibility to radial highways ('rad'), and % lower status of the population ('lstat') have a positive association with the crime rate.
- All the other predictors have a negative association with the crime rate.
- Only Nitric Oxides concentration seems to have a large association with the crime rate.
- Proportion of owner-occupied units built prior to 1940 ('age') and full-value property-tax rate per $10,000 ('tax') have very low association with the crime rate compared to other predictors.
- Proportion of residential land zoned for lots ('zn'), weighted distance to Boston employment centers ('dis'), index of accessibility to radial highways ('rad'), proportion of blacks by town ('black'), and median home value ('medv') have statistically significant relationships with the crime rate.
### Non-linear Regression
- For age, the polynomial terms have statistically significant relationship with the crime rate.
- For tax, only the quadratic term has statistically significant relationship with the crime rate. But cubic term does not have statistically significant relationship with the crime rate.
