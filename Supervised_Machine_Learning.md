# Supervised Machine Learning
1. Regression
2. Classification

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
