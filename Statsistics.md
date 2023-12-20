# STATISTICS
### Descriptive Statistics
### Inferential Statistics
## Probability
## Conditional Probability
## Total Probability Theorem
## Bayes Theorem
## Statistics Distributions
## Discrete Distributions:
 - The sum of all individual probabilities must be equal to one
 - Bernoulis distribution, Binomial distribution, uniform distribution
## Continuous Distribution:
 - The area under the probability curve must be equal to one
 - Normal distribution

### Binomial Distribution:
- Random variables can have only two outcomes  - success/failure or Yes/No
- n random variables
- if n = 1, then binomial distribution is Bernoulli distribution
- The objective is to find the probability of getting k-success out of n trails (k<=n)
- trials should be made up independently
- if the probability of success is p then the probability of failure is 1-p
- If random variables is a Binomial variables, then
   - The trails are independent
   - each trial has either success or failure outcome
   - fixed number of trails
   - the probability of success should be constant
- **Bernoulli distribution**”: One trial or experiment with outcome “success” or “failure”
- ”**Binomial distribution**”: n independent trials, each with outcome “success” or “failure”

### Poisson Distribution:
- we can prefer Poisson distribution, whenever a number of events have to be calculated in a fixed interval of time with a known mean or average rate and independently of the time
### Hypergeometric Distribution

### Uniform Distribution
### Normal Distribution (Gaussian Distribution)
#### Standard Normal Distribution
- mean is zero and variance is 1

### Exponential Distribution

### Chi-square Distribution
- X1, X2,....Xn are normally distributed random variables 
### t-Distribution

## Parametric Test:
- z- test
  - when the sample size is more than 30
  - the population is normally distributed with known variance
  - Testing the value of population mean with the population standard deviation
- t-Test
  - When the sample is less than 30, go with a t-test
  - 
 - F-Test
 - ANOVA

### Non-parametric Test
- Chi-Square test
- Rank Pearson
- Sign Test
- One Sample Ranking
- Spearman's correlation coefficient

### Hypothesis Testing:
- We have to do statistically significant tests in such a way that independent variables do or don't influence the Dependent variables.
- Null Hypothesis - Independent variables do not influence the dependent variable (calculated test value is less than p-value(0.05))
- Alternative Hypothesis - Independent variables influence the dependent variable (The variables are statistically significant)
Error-I = Actual Null Hypothesis is rejected but Null hypothesis is accepted (i.e, Alternate hypothesis has to  be accepted but mistakenly Null Hypothesis is accepted)
Error-II = Actual Alternate Hypothesis has to be accepted but Mistakenly Alternate Hypothesis is rejected



### ANOVA (One-way and Two-way ANOVA)
- F- stats is used to find the relation between two categorical variables
- F-stat = (SSB / DoFB) / (SSW/DoFW)
- SSB = Sum of Squares Between
- SSW = Sum of Squares Within
- SST = Sum of Squares Total =  SSB + SSW
- DOF(T/W/B) = Degree of Freedom (Total / Within/ Between)
- DoF(T) = DoF(B) + DoF(W)
- DoF(T) = (no. of rows * no. of Columns -1)
- DoF(B) = (no. of columns -1)
- 
- R-code for calculating ANOVA
 - aov(dependent varaible ~ independent variable, data)
   
### Association Rule Mining
- support
- Confidence
- Lift

### Karl Pearson's Coefficient of Correlation
- Finding the relation between two variables i.e., how much the variables are related to each other.
- the correlation coefficient (r) = covariance(X,Y) / (std.deviation(X) *std.deviation(Y) )
- -1 < r < 1
- if r = 1; the variables are perfectly  positively correlated
- if r = -1; the variables are perfectly negatively correlated
- if r > 0.75, the variables are highly positively correlated
- 0.3 < r < 0.75, the variables are moderate positive correlated
- 0 < r < 0.3, the variables are weakly correlated


### Spearsman's Rank Correlation Coefficient
- First  rank the variables individually
- Find the difference between the rank of the variables
-  square the difference
-  Formula: R = 1 - (sum of all square of differences / (n *(n^2 - 1)))
-  -1 < R < 1
-  

### Chi-Square Test
- Chi-square is non- parametric test i.e when we are finding the relation between two categorical variables
- Formula = summation of all ((Actual Value - Expected value) ^2 / (Expected Value))
- Degree of Freedom = (column -1) * (Row -1)
- If the calculated value is less than p-value(0.05), reject Null Hypothesis i.e, accept Alternate Hypothesis
