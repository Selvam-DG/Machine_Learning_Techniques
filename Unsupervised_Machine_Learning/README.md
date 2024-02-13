# Unsupervised Machine Learning
## 1. Clustering
- It is also called Segmentation or Grouping
- Only independent variables in the dataset, which means the dataset does not contain the dependent variables
- Based on the feature values, where that particular feature belongs to, is called clustering or grouping.
- Simply
  - Points in a cluster are very close to each other
  - Points in different clusters are far away from each other
- How to measure cluster algorithm performance??
  - K-means cluster 
  - C- means cluster
  - Hierarchical cluster
  - DBSCAN cluster
### K-means Cluster ( Lloyd's Algorithm)
- Algorithm
  - Step 1: Random Intitialisation
    - randomly pick k points from the 'D' dataset and call them C1, C2,....Ck
  - Step 2: Assignment
    - For each point xi in D, select the nearest point (Cj value ) with the help of Euclidean distance (xi, Cj for all points)
  - Step 3: Recompute centroid and update their value
    - recalculate the centroid value of cluster( i,e new values ) and update the Cj value
  - Step 4: Repeat steps 2 and 3 until convergence
    - Euclidean distance between old cluster and new cluster centroid value remains same
- For example, Take two clusters/groups initially C1(20,2) and C2(25,6), and measure the Euclidean distance of new value xi(19,3) concerning two cluster centroids, dist(C1,Xi) =1.414 and dist(C2,xi) =6.7 . so, the minimum Euclidean distance value leads to the respective cluster i.e, xi belongs to the C1 cluster, and the centroid values of that cluster change based on their average C1 (19.5,2.5)
  - https://shabal.in/visuals/kmeans/5.html
- Why Euclidean distance is used in K-means clustering, Why not Manhattan distance??
  - Euclidean distance is the distance between two points, and Manhattan distance is the distance between two points measured along axes at right angles.
  - If the intra-cluster distance is very low, the model is very good, and also the inter-cluster distance is very large, the model is good
- How to choose the cluster number?
  - Use **Elbow method** k-means cluster
### C-means cluster
- If the clusters overlap, then use c-means cluster

- What if the Euclidean distance is the same for both clusters, then use the Hierarchical cluster
### Hierarchical Cluster 
- Also called Dendrogram
- Two methods in Hierarchical cluster.
  1. Agglomarative method 
  2. Divisive method
- **Agglomarative method** is vey popular
  - Total points in the dataset are considered as individual clusters i.e, each point in the dataset is each cluster
  - Then the clusters find the nearest point to their clusters and do this process iteratively to make one cluster
  - Bottom to Top Approach
 ![Screenshot 2024-02-13 180416](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/f6bfef24-e41d-4cf5-8748-4bdb5fcf8f4a)
- 
![An-example-dendrogram-for-the-hierarchical-clustering-shown-in-Table-1-The-original-data](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/335a67e4-10d4-4b10-9294-2bcfd7b46a02)
- Divisive method:
  - In contrast to the agglomerative method
  - It considers maximum value
  - Top Bottom Approach
 ##### K-means cluster is considered centroid based
 ##### Hierarchical cluster considered agglomerative based

 
### DBSCAN - Density-Based Spatial Clustering of Application with Noise
- Can Cluster handle the outlier part??
- In K-means and hierarchical clusters cannot differentiate outlier parts
- Dense Regions
  - Actual cluster data
- Sparse Region
  - Outlier points (noise )
 
- How to measure density??
  - Minpoints, Epsilon, Core-points, board-points, boundary-point, More point, etc.,
#### Measuring Density
- Minpoints and Epsilon values
- Hyperparameter tuning of DBSCAN are Minpoints and Epsilon
- Desnity at point P = number of points within a hyper shape of radius epsilon around P. Here radius value is the Epsilon(€) value and the density (number of points) inside the circle/sphere is called the Minpoint
- Dense Region: It is a hypersphere/circle of radius €(epsilon =1) that contains at least 4 Minpoints
  - Epsilon =1 (radius of the circle is one) and Minpooint is atleast 4, then these are the hyperparameters of DBSCAN
- Sparse region/Noise:
  - If the radius (€) that epsilon is greater than one and Minpoits is less than 4, then it is a Sparse region or outlier
- Core Point:
  - If point p has an epsilon value of one and contains at least 4 Min points around the point within the epsilon value, then that point is called a core point
  - Core points are the same as dense regions 
- Boarder/Boundary Point:
  - IF Point P is not a core point ( which means epsilon value of 1 and Minpoint is less than 4) and Point Q is a core point( epsilon=1, Minpoint >=4 ), P is neighbor of Q if the distance between P and Q is less than or equal to epsilon value(=<1), the P is considered as Border/Boundary point
- Noise point:
  - If a point is Neither a Core point nor a Border  Point, then the point is considered a Noise Point
  - Or else if the epsilon value is greater than 1 and Minpoints is less than 4, or the point is not near of core point, then the point is Noise point

- **DBSCAN algorithm**
  - all data points are labeled as core points, border points, noise points based on hyperparameter tuning epsilon, and minpoints
  - Remove noise points from the dataset (.i,e spare region are removed)
  - for each core point P not assigned to a cluster
    - create a new cluster
    - add all points that are density-connected ( k-d tree = o(log(n) = |D| )
 - Rule of Thumb:
   - Minpoints >= d+1, where d is dimensionality. (Typically Minpoints = 2*d)
   - larger Minpoints, then the dataset is more noise






