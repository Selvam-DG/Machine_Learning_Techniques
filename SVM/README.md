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
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/4e06d048-767c-4ee7-8b9c-de9f650f735e)


## how does it works??
- Identify the right hyper-plane (Scenario-1): Here, we have three hyper-planes (A, B and C). Now,  identify the right hyper-plane to classify star and circle.
- You need to remember a thumb rule to identify the right hyper-plane: “Select the hyper-plane  which segregates the two classes better”. In this scenario, hyper-plane “B” has excellently  performed this job.
- ![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/c04d70e6-11de-42c9-aa4e-652454558d87)

- Identify the right hyper-plane (Scenario-2): Here, we have three hyper-planes (A, B and C) and all aresegregating the classes well. Now, How can we identify the right hyper-plane?
- Here, maximizing the distances between nearest data point (either class) and hyper-plane will help us to  decide the right hyper-plane. This distance is called as Margin.
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/1a2bd327-d6d0-4c53-be62-905d47140cca)
- You can see that the margin for hyper-plane C is high as compared to both A and B. Hence, we name  the right hyper-plane as C. Another lightning reason for selecting the hyper-plane with higher margin is robustness. If we select a hyper-plane having low margin then there is high chance of miss-classification.
- 



### Kernel
- In SVM, it is easy to have a linear hyper-plane between these two classes. But, another burning  question which arises is, should we need to add this feature manually to have a hyper-plane.
No, SVM has a technique called the kernel trick. These are functions which takes low dimensional  input space and transform it to a higher dimensional space i.e. it converts not separable problem  to separable problem, these functions are called kernels.
It is mostly useful in non-linear  separation problem. Simply put, it does some extremely complex data transformations, then find
out the process to separate the data based on the labels or outputs you’ve defined.
![image](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/654fd64c-753f-43e8-8de5-c52dd9b2caac)




