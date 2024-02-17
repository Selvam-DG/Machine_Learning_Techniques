# Cross_Validation
- K-Fold Cross-validation
- K-Fold Cross validation is the typical form of cross-validation
- Approach:
  - Split the training data into 𝑘-folds
  - For each split 𝑖:
    1. Train on all splits, except the 𝑖-th Fold
    2. Evaluate on the 𝑖-th Fold
 - Finally: Average overall results
- When k=1, the process is called Leave-one-out cross-validation (or LOOCV)
- There exist other variants as well, like:
  - Grouped Cross Validation
  - Nested Cross Validation
  - Stratified Cross Validation


# GridSearch CV
- C and gamma values are advanced hyperparameters

# Randomised Search CV
