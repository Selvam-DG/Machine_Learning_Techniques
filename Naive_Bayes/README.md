
## Bayes Theorem
- is one of the most important concept in analysis
- ![download](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/00d19134-779a-445d-a656-316a00705ee5)
- This theorem is used in test analysis, sentimental analysis, and classification
- It is widely used in Natural Language Processing and gives better results
- unsophisticated and simplistic model
![images](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/ab2c171c-db05-42d6-9b45-30d54a26a22e)
- posterior = P(A/B)
- Likelihood = P(B/A)
- prior = P(A)
- Evidence = P(B)


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
