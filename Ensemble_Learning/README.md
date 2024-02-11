# Ensemble Learning
- Collection of Machine Learning algorithms that generate several models (multiple base model[M1, M2,..Mn] from the collection of sample data ) and combine the base model to get the best model
- 4 types of Ensemble Learning
  - Bagging
  - Boosting
  - Stacking
  - Cascading
 
### Bagging
- Boot Strapping Aggregation Method
- Highly performing model and very powerful algorithm
- In real scenarios, the most useful algorithm is Bagging
- It is also called the Learner or Classifier model
- Key aspects:
  - The multiple base models give different results. So combine those models and get a better result out of them
- Core Intuition:
  - A very popular Bagging concept is Random Forest
- Bagging algorithm takes care of high variance and low bias (main idea is to reduce the variance in the dataset)
- Bagging can reduce variance in a model without impacting the bias
  - Model Error/ Generalised Error = Bias^2 +varaiance + Error
- Sampling with replacement to create multiple models
- Bootstrap means the raw data is split into multiple sample data with replacement(row-wise). the model created from the sampling data is Bootstrapping and the multiple sampling data is aggregated/combined to form the Single model is Aggregating.
- In Aggregation, how the model is combined?
  - In classification, the aggregation is based on the multiple model of majority votes
  - In Regression, the aggregation is based on the mean/median of the multiple base model
### Random Forest and their construction
- This is a part of Bagging
- The base model is the Decision Tree
- It is one of the most popular Ensemble methods in which several Tree( Forest) are developed using different sampling strategies like Bootstrapping +Aggregating + feature sampling
- Decision Tree( Base Model) + Bagging ( Row sampling with replacement) + Column Samplig(i.e. feature sampling )
- OOB (Out Of Bag) dataset is the dataset that is not used in any of the models to create the sample models. This OOB data is used for cross-validation of the resulting model.
- **Random Forest = Decision Tree(Base Model) + Row sampling + Column sampling + Aggregation techniques + OOB**
- Feature scaling not required in this algorithm
- cross-validation approach to handle overfitting problem in Random Forest
#### Extremely Randomized Tree
- **Exteemly Randomized tree = Decision Tree(Base Model) + Row sampling + Column sampling + Aggregation techniques + Randomization in selection(tau)** where tau is threshold

## Boosting
- It supported both classification and regression

- In Bagging, If the dataset has high variance and low bias ( in addition to Random Forest i.e column featuring, bootstrapping, and aggregating)
- In contrast, Boosting handles High bias and low variance (bais means train and test model accuracy should be more than 70% and variance means the difference between the train and test model accuracy is less than 15% at most)
- Bagging = Parallel
  - That is sample data from the population data, create multiple models parallelly then finally aggregate to the final model
- Booting = Sequential
  - Create Multiple decision trees sequentially end to leaf node. If the end node gives a negative result, again build a DT
  - weak classification method
    - if the weight is lower, we can train the model with another decision tree
- Boosting method builds a model in sequential order
  - It gives equal weight to all sample datasets
  - find the error weight
  - update the error weight by using the formula (Error = (1/2)*ln((1-TotalError)/total error)
  - error weight = actual weight * exp(new error)

- **Pseudo-residual / False Proxy**
- negative derivative of error = 2* residual i.e dL/dZ = 2*(actual value - predicted value )








### Stacking
- An ensemble learning, Meta-Classifier of stacking
- training dataset -> classified model -> visibility result model -> Meta-Classifier = best accuracy model from the meta classifier
- In stacking, we have the visibility of resulted sample models[M1, M2,...Mn] from the bagging of sample data and, choose the best model which gives the best accuracy. This is meta classifier. Here no aggregation concept, because the sample model output can be visible
- Computation time is more compared to other ensemble techniques because stacking involves all other models( logistic regression, KNN, NaiveBayes ...... )














