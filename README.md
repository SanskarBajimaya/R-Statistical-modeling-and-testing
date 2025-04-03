# R-Statistical-modeling-and-testing
R statistics from John Hopkins University Course <br>

# Project Overview
This project analyzes the relationship between transmission type (automatic vs. manual) and miles per gallon (MPG) using the mtcars dataset. The goal is to determine which transmission type is more fuel-efficient and quantify the difference.

# Key Sections
## 1.	Exploratory Data Analysis (EDA): 
Descriptive statistics, visualizations, and correlation analysis.
## 2.	Model Selection: 
Simple and multiple linear regression models to compare MPG between transmission types.
## 3.	Model Diagnostics: 
Residual analysis, multicollinearity checks, and assumption validation.
## 4.	Inference: 
Confidence intervals, hypothesis testing, and bootstrap analysis.
## 5.	
Conclusion: Summary of findings, implications, and limitations.

## Results
Taking every test account, we can say that the fit3 [lm(mpg~am + hp + wt, data = mtcars)] might be our best preference as it has passed anova test with good F-stats and P values, multi-collinarity test with appropriate variance influence factor, has higher adjusted R squared value and have lowest AIC and BIC values. <br><br>
We see that at 95% confidence level, the effect of changing from automatic to manual transmission on "mpg", an increase of -0.258 to 4.121 mpg. However as there is 0 falling in the range, we can suggest that our model accuracy is not so strong at 95% confidence level as the change in transmission can have zero change in mpg. <br> <br>
We see that at 85% confidence level, the effect of changing from automatic to manual transmission on "mpg", an increase of 0.046 to 4.121 mpg. This shows that our model is not accurate enough at predicting the relationship of change in transmission and change in mpg at higher signficance level. 

Model Used: Multiple linear regression with covariates horsepower and weight.
