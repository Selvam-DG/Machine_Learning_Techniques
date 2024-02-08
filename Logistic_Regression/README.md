# Logistic Regression
- result variable /Dependent variable is categorical or dichotomous 
- Dependent variable is a binary class(yes/No, True/False, 0/1) then use logistic regression
- sigmoid function
- with the sigmoid function, the range becomes (0, infinity)
- Apply logarithm, then the range changes to (-infinity to + infinity)
- ln(p/(1-p)) = Y = beta0 + beta1*X1 + beta2*X2 +...... + Error
- odds = success/ failure
- logit = logarithm( odds)
- If the dependent variable is multi-class, don't use Logistic regression.
### Geometrical Intuition:
- If data is linearly separable (almost linearly separable) - that is data is divided into two types (yes/no, high/low, 0/1 .....)
- Divide the data into two types with the separable line so-called hyper (pi) plane

## Performance metrics:
- Accuracy = # correctly classified points / Total # points in the dataset
- confusion matrix = TrueNegative(TN), FalseNegative(FN),FalsePositive(FP), TruePositive(TP)
  - P\A  0	   1
  -  0	  TN	   FN
  -  1	  FP	   TP
- TPR(True Positive Rate) =  TP/P =TP /(FN+TP)
- TNR(True Negative Rate) = TN/N = TN / (TN+ FP)
- FPR = FP/ N = FP/ (TN + FP )
- FNR = FN/ P = FN / (FN+ TP )
- Recall/sensitivity = TPR = is nothing but the from all of the actual positive points, how much percentage of them are predicted by the model is correctly
- Precision = TP/(TP+FP) = from the positive values predicted by the model, what percentage of them are positive actually in the original dataset.
- Error = (FP + FN) / (TN + FN + FP + TP) 
- Accuracy = (TP + TN) / (TN + FN + FP + TP) 
-  F1-stats = 2 * ((Precision*Recall)/ (Precision + Recall))
-  ROC = Receiver Operating characteristics
    - The plot of TRP Vs FPR and the constant line is called Area under the curve
    - The line above AUC is called Receiver Operating Characteristics
    - If predict values are Fewer false values and more True values, then the model is good
    - CASE1: If ROC curve go above the AUC( threshold line ), then model is good
    - CASE 2: If ROC curve on the AUC (threshold line ), then the model is appropriate -> imbalance dataset
    - CASE 3: If ROC curve is under the AUC line, then the model is not good
![download](https://github.com/Selvam-DG/Machine_Learning_Techniques/assets/98681717/52c442d6-92c0-4242-8620-197cae188c5e)

-  AUC = Area Under Curve
-  

-  
