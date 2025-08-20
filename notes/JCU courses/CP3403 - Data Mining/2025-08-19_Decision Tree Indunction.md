---
date: "2025-08-19"
location: 
    - JCU courses/CP3403 - Data Mining
hubs: 
    - "[[]]"
urls:
    - 
---

# Decision Tree Indunction
## Basic algorithm
+ Type: Greedy / top-down recursive / divide-and-conquer
+ Start all train examples - are roots
+ All attributes MUST be categorical (discretize beforehand)
## Condition to stop
+ All samples belong **same** class
+ No remaining attributes
+ No samples left

## Extract tules
+ Form: IF-THEN rules
+ One path - One rule
+ One attribute-value pair - conjuction
+ One leaf node - One prediction

## Strengths
+ Comprehensive
+ Applied to real-life
+ Make no prior assumptions
+ Work both numerical / categorical data
+ Faster than Neural Networks

## Weaknesses
+ Output MUST be categorical 
+ Limited to one output attribute
+ Are unstable
+ Trees can become complex
