# Pricipal Component Analysis (PCA)
- This is the dimensionality reduction method
- This method is applicable for both supervised and unsupervised Machine Learning
- If we have a huge data set or many variables are there in the dataset, we use dimensionality reduction
  - The reduction may be variables( columns) or values that are non-significant to the dataset
  - The reduction handles multicollinearity by removing redundant features, handling missing values, outliers
  - This reduction is not targeted to non-significant variables, we can target particular value
 
- PCA takes less tunning and computational time
### Eigen Values and Eigen Vector
- This eigenvalue and eigenvector concept is used in several ML models and algorithm
  - PCA
  - Factor Analysis
  - Reinforcement Learning


- Summary of Algorithm
  1. Find principal directions 𝑤1,…𝑤𝑝 and eigenvalues 𝜆1,…,𝜆𝑝
  2. Project data points into new coordinate frame using 𝑻 =𝑿𝑾
  3. Keep the 𝑞 most important dimensions as determined by 𝜆1,…,𝜆𝑝(which are sorted by variance)
 
- Summary of Principal Component Analysis
  - Rotate the coordinate system such that all axes are sorted from most variance to least variance
  - Required axes 𝑾 determined using either
    - Eigenvectors and –values of covariance matrix 𝑪 = 𝑾𝑳𝑾𝑇
    - Singular Value Decomposition (SVD) of data points 𝑿 = 𝑼𝑺𝑾𝑇
  - Subsequently, drop axes with the least variance
  - Variance-based feature selection has limitations
 









source: FAU university
