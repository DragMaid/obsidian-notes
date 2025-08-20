---
date: "2025-06-09"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Classification Accuracy
=> Classification accuracy = (TP + TN) / (TP + FP + FN + TN)

# [[Contigency table]]
# [[Sensitivity]] (recall) (TP rate)
# [[Specificity]]
# [[Recall]]
# [[Precision]]

## Example 1
+ Use case: If you want to find every person with a disease then use [[2025-06-09_Sensitivity|sensitivity]]
+ Reason: This is because a false negative is very bad !! (especially for infectious diseases)
    + The doctor says you don't have cancer -> die of cancer since couldn't cure it soon
    + The FP tends to be very large (better to get 100 healthy people re-checked than to let a single sick person untreated)

## Example 2
+ Use case: if you don't want to find every person with a disease but want to avoid false positives use [[2025-06-09_Precision|precision]]
+ Why: oftene used in marketing problems
    + Database has millions -> can't phone all
    + Want a classifier that 99% of them will buy -> want low FP

# [[Error Rate Estimation]]

# [[ROC Curves]]

# [[No free lunch Theorem]]

# [[Issues about classifaction]]

# [[Evaluating Classification Methods]]
