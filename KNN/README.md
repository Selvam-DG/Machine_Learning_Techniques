# K-Nearest Neighbor
- hyper parameter (k value) to get the nearest value
- k value is always odd value
- Failure cases of KNN:
  - far away points are cannot be decided
  - Jumble of data is not possible with KNN
### KNN Algorithm
 - Choose K
 - Find Distance with all point from test point
   -  Euclidean Distance = sqrt(sum((x- y)^2)) = sqrt((𝑥1 − 𝑥2)^2+(𝑦1 − 𝑦2)^2)
   - Manhattan Distance = sum(|x- y|)
   - Chebyshev Distance = max(|x- y|)
   - Minkowski Distance = sum(|x- y|^p)^(1/p)
   - WMinkowski Distance = sum(|w * (x- y)|^p)^(1/p)
   - SEuclidean Distance = sqrt(sum((x- y)^2 / V))
   - Mahalanobis Distance = sqrt((x- y)' V^-1 (x- y))

 - Sort Distance
 - Select K point with Minimum distance
 - Classify in majority vote

### Some Aspect of KNN
 - Lazy learner
 - Instance Based
 - Just memorization of Data
 - Easy interpretation of result
 - Performance on Read world data – not very good
 - Computational cost very high for big dataset
 - Non-parametric in nature
