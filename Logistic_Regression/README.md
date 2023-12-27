# Logistic Regression
- Out variable/ result variable /Dependent variable is categorical or dichotomous 
- Dependent variable is a binary class(yes/No, True/False, 0/1) then use logistic regression
- sigmoid function
- with the sigmoid function, the range becomes (0, infinity)
- Apply logarithm, then the range changes to (-infinity to + infinity)
- ln(p/(1-p) = Y = beta0 + beta1*X1 + beta2*X2 +...... + Error

### Geometrical Intuition:
- If data is linearly separable (almost linearly separable) - that is data is divided into two types (yes/no, high/low, 0/1 .....)
- Divide the data into two types with the separable line so-called hyper (pi) plane

## Performance metrics:
- Accuracy = # correctly classified points / Total # points in the dataset
- confusion matrix = TrueNegative(TN), FalseNegative(FN),FalsePositive(FP), TruePositive(TP)
- 0	1
0	TN	FP
1	FN	TP
- TPR(True Positive Rate) = TP /(FN+TP)
- TNR(True Negative Rate) = TN / (TN+ FP)
- FPR
- FNR
- Recall/sensitivity = TPR = is nothing but the from all of the actual positive points, how much percentage of them are actually predicted by the model
- Precision = TP/(TP+FP) = from the positive values predicted by the model, what percentage of them are actually positive
- Error = (FP + FN) / (TN + FN + FP + TP) 
- Accuracy = (TP + TN) / (TN + FN + FP + TP) 
-  F1-stats = 2 * ((Precision*Recall)/ (Precision + Recall))
-  ROC =
-  AUC =
-  

-  
