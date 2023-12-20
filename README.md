# Machine Learning and Algorithms
### Supervised Machine Learning
- Regression
- Classification
### Unsupervised Machine Learning
- Clustering / Segmentation / Grouping
- Recommendation Engine/ Market Basket Analysis
### Re-inforced Machine Learning
- Penalty
- Reward
### Semi-Supervised Machine Learning

- Supervised ML methods have Independent and Dependent Variables. Split the data into train and test and then predict the values with test data with actual data
- Unsupervised ML methods have only an independent variable (NO target variable) and no data splitting

#### Regression
-  Dependent and Independent variable
- Dependent variables is a continuous changeable variable, then the model comes under Regression
- Algorithms
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - Support Vector Machine Regressor
  - K - Nearest Neighbour KNN Regressor
  - Ensemble Learning Regressor

#### Classification
- Binary/Multiclass/Categorical/Dichotomous problem
- the problem having a solution of yes or no / True or False/ 0 or 1 -  those problems come under Classification problem
- Algorithms:
   - Logistic Regression
   - Decision Tree Classifier
   - Random Forest Classifier
   - Support Vector Machine Classifier
     - Kernel => Linear/ Sigmoid/ Polynomial / Radial Basial Function
   - K Nearest Neighbour KNN => Naive Base Theorem
   - Ensemble Learning
 
#### Ensemble learning
- Support both Regression and classification problem
- 4 types of Ensemble
  - Bagging
    - Bagging
    - Random Forest
  - Boosting
     - Ada Boost
     - Gradient Boosting
     - XG Boosting (Extra Gradient Boost)
     - Light GBM Boosting
     - Cat Boosting
  - Stacking
  - Cascading

#### Clustering / Segmentation / Grouping
- Cluster or Group the data into similar classes and targeting the most efficient cluster of data is simply a clustering technique
- Algorithms:
  - K- means Cluster
  - C - means Cluster
  - Hierarchical Cluster
  - DBSCAN (Density-Based Special Cluster of Application Noise)
#### Association Rule Mining / Market Basket Analysis
- Coupons offered in shop or production suggestions while shopping in online are the example of Association Rule Mining
- Algorithm:
  - Apriore

#### Time Series Forecasting
- Here, problems are done in 2 ways
1. Machine Learning
  - ARIMA (Auto Regressive Integrated Moving Average, AR- Auto-Regressive, MV- Moving Average, SARIMA
2. Deep Learning
  - LSTM ( Long Short Term Memory)
- when data containing time and date and are independent variables affecting the output variable, then the Time Forecasting Algorithm is used

Model: 
- Actual fitting => if train data gives 90% then test data(predict) gives 90% result
- Underfitting=> 50% train data(Building data) and 50% test data(predict data) = High Bias (Prefer Algorithm  XG Boost)
- Overfitting => 90% train data and 50% test data = High Variance (Prefer Algorithm - Random Forest) 
