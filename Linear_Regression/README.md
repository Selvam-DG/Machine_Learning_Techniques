# Supervised Machine Learning
1. Regression
2. Classification

# Regression :
- Dataset contains features (independent variables ) and the label outputs (dependent variables)
- The problem has to be simple:
  - The dataset is small
  - Linear model is enough i.e. Trend Analysis
  - Linear models are the basis for complex models i.e. Deep Networks
- Regression Model Fit:
  - Linear model
  - Polynomial model
  - Gaussian model

    
## Assumptions for Linear Regression Model
1. Data should be linear
2. Data should be normally distributed
3. There should not be any Heteroscadicity (data should not contain outliers)
   - Outliers are highly significant in Linear regression algorithm
4. There should not be any auto-correlation
   - The predicted dependent variable is same of two independent factors  
   - This is checked by the Durbin-Watson Test (Range is 0 to 4)
   - If Durbin Watson Test = 2, No Auto-correlation
   - if 0 < Durbin Watson Test <2 , postive correlation
   - if 2 > Durbin Watson Test > 4, then data contain a negative correlation
   - check p_value, if the Durbin-Watson Test lies between 1.5 to 2.5. If the p_value is less than 0.05, then consider the variable
   - if the Durbin Watson Test < 1.5 or Durbin Watson Test > 2.5, reject the Linear Regression model, do the data analysis with time series forecasting
5. Data should not contain any multicollinearity (i.e no two  independent variables should not be  strongly correlated)
   - Check multicollinearity with the help of Heatmap and check the correlation
   - Another method to check multicollinearity is Variance Inflation Factor (VIF)
     - if the Variance Inflation Factor is more than 5, then the data contain multicollinearity
     - drop the variable and build the model
6. Select the right dependent variable which is the so-called Endogeneity

**Result prediction**
8. R-square is the coefficient of determination.
   - It is a measure of the percentage of variability of the dependent variable (𝐲) in the data explained by the model!
9. check R_square, adjusted R_square( Threshold is 0.7) - check the adjusted R square values which consider only significant variables whereas the R square considers both significant and non-significant variables.
10. Check the p_value of all independent variables (should be less than 0.05)



- Three Phases 
  - Geometrical Intuition
  - Probabilistic Approach
  - Log-Loss function

- If Dataset D(Xi,Yi) contains one independent and one dependent variable, then it is a simple linear Regression
- If the Dataset contains  more than one independent variable and one dependent variable, then it is a multiple linear regression
- If the dependent variable is a continuous variable of the Real number with an n-dimension
- If the dependent variable is (0,1), then it is a classification  Problem (eg: yes/no, True/ False, Buy/Not Buy......)
- If dependent variable is in range of(0,9), then it multi-class classification problem (eg. Rating the product, 
- if the dependent variable belongs to the Real number with n dimension, then it is a regression






### Error / Loss / Cost
- Square Loss Function = difference of Predicted value from  Actual value
- The best-fit line in Linear Regression to get a minimum error (i.e, a minimum value of summation of squares of(actual value - expected value)
- The algorithm used in  the Linear Regression Model is **Ordinary Least Square (OLS)/Linear Least Square(LLS)/Square Loss Function**
- OLS = argmin(summation of all (Actual value - Expected value)^2)
### Regularization Approach (Optimization)
- Balancing the dataset to the same scale is regularisation
- Regularisation is used to remove overfitting or underfitting problem
- used to avoid overfitting(high variance) and underfitting(high bias) problems
- L2-Regularisation = Lasso (High value) - Overfit problem (i.e the training accuracy is more and test accuracy is less )
- L1-Regularisation = Ridge (Low value) - underfit problem (i.e, training accuracy and test accuracy both are less than 50% )
- L1 + L2 - regularisation = ElasticNet

### Measurement to find data accuracy in Data Science
- MAE  Mean Absolute Error
- MAPE= Mean Absolute Percent Error
- MSE = Mean Square Error
- RMSE = Root Mean Square Error
- AIC = Akike Information Criterion
- BIC = Basian Information Criterion



#### Mean Absolute Error (MAE):
- Average difference between the original and predicted values
- Measure how far predictions were from the actual output 
- Does not give an idea about the direction of error

#### Mean Squared Error (MSE):
 • Similar to MAE
 • It takes the average of the square of the difference between the original and predicted value
 • Larger errors become more pronounced so that the model can focus on larger errors.

