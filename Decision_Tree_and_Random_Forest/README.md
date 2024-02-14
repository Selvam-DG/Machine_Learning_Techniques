## Decision Tree
- Supervised Machine Learning algorithm
- Classification Tree
- Regression Tree
- Discrete and continuous dependent variable
- If the outcome/ dependent variable is discrete, then it is a classification tree
- If the outcome variable is continuous, then it is a Regression tree
- Geometrical intuition in the Decision Tree algorithm is **Axis Parallel Hyperplane**
- Decision Tree is simply a nested if-else condition
#####################################################################################################################################################################
- Root Node:
  - Starting of the decision tree
- Branch Node:
  - split into branches with 2 or more branches
- Leaf Node
  - End point of the decision tree
### Why Decision Tree?
- Decision trees are powerful and popular tools for classification and prediction.
- Decision trees represent rules, which can be understood by humans
- Relatively fast compared to other classification models
- Obtain similar and sometimes better accuracy compared to other models 

### How does a tree decide where to split?
- Gini Index
- Entropy
- Chi-Square
- Information Gain
- Reduction in Variance

**Gini Index** : 
  - GI = p^2 + q^2 ,  where p = success and q = failure
  -  It works with categorical target variable “Success” or “Failure”
  -  It performs only Binary splits
  -  The higher the value of Gini, the higher the homogeneity
  -  CART (Classification and Regression Tree) uses Gini method to create binary splits

**Entropy**:
  - Entropy = -p*log(p) -q*log(q),  where p = success and q = failure
  - The lesser the entropy value, the better the root node
**Chi-Square**
  - summation of square of (actual value- predicted value) / actual value
**Information Gain**:
  - Information Gain = 1 – Entropy
  - Here, p and q is the probability of success and failure respectively in that node.
  - Entropy is also used with categorical target variables.
  - It chooses the split which has the lowest entropy compared to parent node and other splits.
  - The lesser the entropy, the better it is.
  - Calculate entropy of parent node
  - Calculate the entropy of each individual node of split and calculate the weighted average of all subnodes available in split.

### Benefits of Decision Tree:
1. Rule generated are simple( nested if-else condition) and interpretable (Geometric- Axis parallel hyperplane )
2. Tree can be visualized
3. The Decision Tree algorithm works well with both numerical and categorical data
4. Rule can help to create a business strategy

- Outlier and feature scaling is not required in Decision tree
- regression - we don't need to check the imbalance dataset

### Preventing Overfitting:
- By setting constraints on

# Random Forest
- Random Forest algorithm is a multiple decision tree algorithm


### OOB Error rate

