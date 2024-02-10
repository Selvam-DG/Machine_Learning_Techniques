# K-Nearest Neighbor
- hyperparameter (k value) to get the nearest value
- k value is always an odd value
- Failure cases of KNN:
  - far away points cannot be decided
  - A jumble of data is not possible with KNN
### KNN Algorithm
 - Choose K
 - Find Distance with all points from test point
   - Euclidean Distance = sqrt(sum((x- y)^2)) = sqrt((𝑥1 − 𝑥2)^2+(𝑦1 − 𝑦2)^2)
   - Manhattan Distance = sum(|x- y|)
   - Chebyshev Distance = max(|x- y|)
   - Minkowski Distance = sum(|x- y|^p)^(1/p)
   - WMinkowski Distance = sum(|w * (x- y)|^p)^(1/p)
   - SEuclidean Distance = sqrt(sum((x- y)^2 / V))
   - Mahalanobis Distance = sqrt((x- y)' V^-1 (x- y))
 - Sort Distance
 - Select K point with Minimum distance
 - Classify in majority vote

### Some Aspects of KNN
 - Lazy learner
 - Instance-Based
 - Just memorization of Data
 - Easy interpretation of the result
 - Performance on Read world data – not very good
 - Computational cost very high for big dataset
 - Non-parametric in nature



- L2-Norms: ||x1 - x2|| = summation of euclidean distance
- L1-Norms : Manhattan Distance = summation of absolute difference(distance between two points) = |x1-x2|
- LP-Norms or P-Norms: Minkowski distance = summation of(|x- y|^p)^(1/p)
  - If p =1 in Minkowski distance, then it is Manhattan distance = L1-Norms
  - If p =2 in Minkowski distance, then it is Euclidean distance = L2-Norms
- Jaccard Distance:
  - J(A,B) = |A intersection B| / |A union B |
- Cosine distance:
  - cos theta = vector product of a,b divided by product of unit vector of a,b 
![hqdefault](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/8833fc1d-c7eb-4e4d-9bf7-12e55b7f3961)
- Hamming Distance (boolean vector)
  - will use this, if the dataset is a boolean or categorical dependent variable
-The Hamming distance between two codewords is defined as the number of elements in which they differ. The minimum distance dmin of a linear block code is the smallest Hamming distance between any two different codewords, and is equal to the minimum Hamming weight of the non-zero codewords in the code.
![download](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/a095d31e-9eaf-474e-b834-7fb516f0a6d9)



### Steps
- Importing Library and Load Data
- Normalize Data - scaling
- Split data – Train Test
- Apply KNN on 1 Test  Sample
- Accuracy









