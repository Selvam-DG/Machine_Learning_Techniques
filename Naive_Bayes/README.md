
## Bayes Theorem
- is one of the most important concepts in analysis
- ![download](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/00d19134-779a-445d-a656-316a00705ee5)
- This theorem is used in text analytics, sentimental analytics, and classification
- It is widely used in Natural Language Processing and gives better results
- unsophisticated and simplistic model
![images](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/ab2c171c-db05-42d6-9b45-30d54a26a22e)
- posterior = P(A/B)
- Likelihood = P(B/A)
- prior = P(A)
- Evidence = P(B)

![Screenshot 2024-02-11 151052](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/c1eac4c1-258c-4ca8-9c44-cb0344c3c047)
## Handling missing values in Naive-Bayes
- Text- Data
  - Naive Bayes algorithm didn't  handle missing values, we'll leave the missing values
  - we cannot consider missing value if the data is text
- Categorical features
  - Missing values are considered as NaN
  - NaN is considered as category
  - NaN are replaced by MODE (Most Frequent Approach)
- Numerical features
  - Imputation techniques (such as mean or median) based on Outliers
  - If outliers are found in the Dataset, use the Median
  - If no Outliers are found, use Mean to fill the missing values (NaN values)
##### Can Multi-class classification handled by NaiveBayes??
- Yes, NB can do multiclass classification
- NB cannot handle the Regression Problem
#### Can NB handle the similarity matrix/ Distance Matrix ??
  - Distance or similarity matrix can be seen in the KNN algorithm
  - So, NB cannot used in distance or similarity matrix or distance-based method
 
- Naive Bayes is a probability approach

#### Can Naive Bayes handle Large Multidimensionality?
- Yes, NB handle Multidimensionality
- Text analytics must contain high dimensions, so NB can handle multidimensionality
- **log-probabilistic approach** which is a numerical stability
  - Log probabilities for numerical stability
![Screenshot 2024-02-11 141510](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/f957344c-cd70-4349-aae8-cd170428cab8)

- Best and Worst cases of Naive Bayes:
  - Conditional independence of features (in  classification problem )

    - IF conditional probability gives a true result, NB performs very well as per the theory
    - If condition probability gives a false result, then NB deteriorates or degrades
  - Text- classification
    - Example is spam/ ham mail
    - 
  - Categorical features
    - Machine learning with classification problems, don't use Gaussian Naive Bayes method
    - If time is critical to complete the model, then use Gaussian Naive Bayes algorithm to complete the model
  - Interpretable method and feature impotence method
    - Less run time, train time and test time are low, run time space is also less
    - so NB is very simple to implement
  - NB is easily overfitted if don't do the Laplace smoothing
  
**Laplace / Additive Smoothing**
-   alpha=1, k=2 where alpha is Laplace smoothing and K is the number of distinct values that an unknown variable can take
-   function = ( # datapoint + alpha) / (total number of data points + (alpha*K))
-   Hyperparameters used in Naive Bayes theorem are alpha and k
-   

  
- 
