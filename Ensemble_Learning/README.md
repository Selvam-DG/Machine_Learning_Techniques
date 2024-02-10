# Ensemble Learning
- Collection of Machine Learning algorithms that generate several models (multiple base model[M1,M2,..Mn] from the collection of sample data ) and combine the base model to get the best model
- 4Types of Ensemble Learning
  - Bagging
  - Boosting
  - Stacking
  - Cascading
 
### Bagging
- Boot Strapping Aggregation Method
- Higlhly performing model and very powerful algorithm
- In real scenarios, the most useful algorithm is Bagging
- It is also called Learner or Classifier model
- Key aspects:
  - The multiple base models give different results. So combine those models and get the better result out of them
- Core Intuition:
  - very popular Bagging concept is Random Forest
- Bagging algorithm is taking care of high variance and low bias (main idea is to reduce the variance in the dataset)
- Bagging can reduce variance in a model without impacting the bias
  - Model Error/ Generalised Error = Bias^2 +varaiance + Error
- Sampling with replacement to create multiple model
- Bootstrap means the raw data is splitted into multiple sample data with replacement(row wise). the model created from the sampling data is Bootstrapping and the multiple sampling data is aggregate/ combine to form the Single model is Agrregating.
- In Aggregation, how model is combinig?
  - In classification, the aggregation is based on the multiple model of majority votes
  - In Regression, the aggregation is based on the mean/median of the mutliple base model
### Random Forest and their construction
- This is a part of Bagging
- Base model is Decision Tree
- It is one of the most popular Ensemble method in which several Tree( Forest) are developed using different sampling strategy like Bootstrapping +Aggregating + feature sampling
- 
