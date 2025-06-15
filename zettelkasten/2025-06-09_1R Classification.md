---
date: "2025-06-09"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# 1R Classification
+ Simple - but effective
+ One attrivute might do all work
+ 1-level decision tree -> generate rules tested on 1 attribute
+ Choose attribute with lowest error rate

## Procedure
+ For each attribute
    + Count how often each class appears
    + Find most frequent class
    + Make rule assign that class to this attr-value
- Calculate the error rate of the rules
+ Choose rules with min(error rate)

![[Pasted image 20250609184417.png]]