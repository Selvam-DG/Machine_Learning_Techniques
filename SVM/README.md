# Support Vector Machine (SVM)
- one of the most popular and talked about machine learning algorithms
- go-to method for a high-performing algorithm with little tuning
- developed in the 1990s
- A sophisticated idea but has a simple implementation
### What is SVM?
- A supervised machine learning algorithm that can be used for both classification and regression and outlier detection
- Considered to be a classification approach, generally.
- SVMs are based on the idea of finding a hyperplane.
- SVM constructs a hyperplane in multidimensional space to separate different classes
- SVM generates optimal hyperplane in an iterative manner
- Find a maximum marginal hyperplane(MMH) that best divides the dataset into classes – widest street approach
- Handles both the continuous and categorical variables.



## how does it works??
- Identify the right hyper-plane (Scenario-1): Here, we have three hyper-planes (A, B and C). Now,  identify the right hyper-plane to classify star and circle.
- You need to remember a thumb rule to identify the right hyper-plane: “Select the hyper-plane  which segregates the two classes better”. In this scenario, hyper-plane “B” has excellently  performed this job.
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/b93d0b10-fc4c-4dec-be13-836c0052ea72)


- Identify the right hyper-plane (Scenario-2): Here, we have three hyper-planes (A, B and C) and all aresegregating the classes well. Now, How can we identify the right hyper-plane?
- Here, maximizing the distances between nearest data point (either class) and hyper-plane will help us to  decide the right hyper-plane. This distance is called as Margin.
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/2bdabf1c-5f98-4516-89b4-c48a83cd8671)

- You can see that the margin for hyper-plane C is high as compared to both A and B. Hence, we name  the right hyper-plane as C. Another lightning reason for selecting the hyper-plane with higher margin is robustness. If we select a hyper-plane having low margin then there is high chance of miss-classification.
- Can we classify two classes (Scenario-3)?: Below, I am unable to segregate the two classes using  a straight line, as one of star lies in the territory of other(circle) class as an outlier.
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/eda4d8c3-4c1c-4fb0-b908-2e8c66319303)
- As already mentioned, one star at other end is like an outlier for star class. SVM has a feature to  ignore outliers and find the hyper-plane that has maximum margin. Hence, we can say, SVM is  robust to outliers.
-Find the hyper-plane to segregate to classes (Scenario-5): In the scenario below, we can’t have  linear hyper-plane between the two classes, so how does SVM classify these two classes? Till  now, we have only looked at the linear hyper-plane.
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/d11e81db-bb3d-4ccf-b283-9a3d4252aa16)
- SVM can solve this problem. Easily! It solves this problem by introducing additional feature. Here,we will add a new feature z=x^2+y^2. Now, let’s plot the data points on axis x and z.







### Kernel
- In SVM, it is easy to have a linear hyper-plane between these two classes. But, another burning  question which arises is, should we need to add this feature manually to have a hyper-plane.
No, SVM has a technique called the kernel trick. These are functions which takes low dimensional  input space and transform it to a higher dimensional space i.e. it converts not separable problem  to separable problem, these functions are called kernels.
It is mostly useful in non-linear  separation problem. Simply put, it does some extremely complex data transformations, then find
out the process to separate the data based on the labels or outputs you’ve defined.
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/d83a16a9-a232-4d98-942b-f94ac0aa8c81)

### Pros and Cons:
- It works really well with clear margin of separation
- It is effective in high-dimensional spaces.
- It is effective in cases where a number of dimensions is greater than the number of samples.
- It uses a subset of training points in the decision function (called support vectors), so it is also memory efficient.
Cons:
- It doesn’t perform well, when we have a large data set because the required training time is higher
- It also doesn’t perform very well, when the data set has more noise i.e. target classes are  overlapping





