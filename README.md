# MechaCar_Statistical_Analysis

## Overview of the project
In this project we did a business analysis of a new MechaCar Prototype that is having production troubles and that's affecting the company's manufacturing team’s progress. In order to perform the analysis we used the production data to determine the best decision to solve this problem.
### Analysis Overview

In this analysis we include the following:

- Linear regression to determine the variables in the dataset predict the mpg of MechaCar prototypes.
- Summary statistics on the pounds per square inch (PSI) of the suspension coils from the manufacturing lots.
- T-tests to determine if the manufacturing lots are statistically different from the mean population.

### Programs used

- R, Rstudio and R dplyr library 
- Datasets can be found in the Rstudio folder. 

## Analysis
### Linear Regression
1.According to the following tables we can see that the variables that provide the most non-random amount of variance are the Spoiler Angle, Vehicle Weight and the AWD. 

2.The slope of the model is not zero because p-value is 5.35x10^-11. We know this because the standard is 0.05 and the value that we found is considerably lower. Therefore we can safely conclude that the response variables are correlated to the predictor variable. 

3.Does this linear model predict MPG of MechaCar Prototypes? Like in any model, there is always room for improvement and there is more statistical test that could make this analysis more robust. Nonetheless we can determine that this model is strong but it could be better. We have a value of R-squared of 0.71. There might be external or internal factors that could affect the value of the R-squared. 
![](/resources/coefficients.png)
![](/resources/linearRegression.png)

### Summary Statistic on the PSI of the Suspension Coils
Do the design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually?

- Lots 1 and 2 meet the required standards.
- Lot 3 does not meet the required specifications because it's variance has a value of 170.28
![](/resources/lots_summary.png)
![](/resources/total_summary.png)

### T-tests
We used T-tests to determine the significance of the analysis performed on the lots. The results were: 
- In the first t-test we have a p-value of 0.060 which is slightly bigger than the significance level of 0.05. We could determine that the distribution normal.
- The p-value for Lot 1 is 1, so the distribution is normal.
- The p-value for lot 2 is 0.06, so the distribution is normal. 
- The p-value for lot 3 is 0.04, lower than our significance level of 0.05. Therefore we can determine that the distribution is not normal.


![](/resources/t_tests.png)

## MechaCar vs Competition

According to www.drive-safely.net one of the most important things for drivers when buying a car is safety and other source, www.protectiveagency.com, concluded that cost and financing are other important factors. With this information we can perform a study where we compare the prices of the competitors to our prices. Then for the safety part of the study we need to set a required safety rating, do various tests where we compare different models of prototypes, gather the information in a data set and determine what prototypes passed the test. After this we would need to perform a statistical t-test where we state a hypotheis and calculate if our dataset is correct and can predict the safety of our cars. One example of a null hypothesis for the safety test may be:
- The prototypes of lot 1 meet the required safety rating. 
