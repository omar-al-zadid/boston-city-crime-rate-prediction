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
- All the predictors except for 'chas' (represents tracts binding the river)  have statistically significant relationship with the response.
- 'Nox' representing nitric oxide concentration has a large positive association with the per capita crime rate.
- The predictor 'rm' representing average number of rooms per dwelling has a negative small association with the crime rate per capita.
- The predictor 'dis' representing weighted distance to Boston employment centers has a negative small association with the crime rate per capita.
- 'Medv' denoting median home value has a negative small association with the crime rate per capita.
- Though the coefficients are unstandardized, only nox seems to have a large association with the crime rate.
- All other predictors seem to have a smaller association with the crime rate.
